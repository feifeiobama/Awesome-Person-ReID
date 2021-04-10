* 
* (PAMI 2015) Map-Based Probabilistic Visual Self-Localization
  * map representation: node: street, state: u~t~ (unknown), s~t~
  * ==GMM on s~t~: $\mu,\Sigma$ ==
  * filter: predict, update
* (IJCAI 2016) A Collaborative Filtering Approach to Citywide Human Mobility Completion from Sparse Call Records
  * ==HMM based completion== ( trajectory smoothing)
* (PAMI 2017) Geometric Graph Matching Using Monte Carlo Tree Search
  * graph matching by measuring total length of matched superedges
  * Mento Carlo Tree Search (==incremental==)
* (KDD 2014) Travel Time Estimation of a Path using Sparse Trajectories
  * deal with sparsity by 3d tensor decomposition
  * optimal ==concatenation by dynamic programming==
* (TCS 2006) Correlation clustering in general weighted graphs
  * ==linear programming== to give a fractional solution
  * round to an integral solution
* (SDM 2017) Robust Map Matching for Heterogeneous Data via Dominance Decompositions
  * find dominance decompositions
* (SIGSPATIAL 2016) Knowledge-Based Trajectory Completion from Sparse GPS Samples
  * skeleton -> branch: L-shape interpolation)
  * junction (vertices: minimum trajectory flow)
  * trajectory completion: fill gap: k-nearest & cosine similarity (spatial)
* (TVCG 2015) TrajGraph: A Graph-Based Visual Analytics Approach to Studying Urban Network Centralities Using Taxi Trajectory Data
  * edges: street length, number of transition, average travel time, average speed
  * refine: DBSCAN
  * high pagerank / high betweenness refer to ...
* 

#### 想法

作为 Map matching 问题

* 许多短片段很难进行推断，在单摄像头内进行推断（DP/MCTS），重新构建id

* 补全相似度较低的时空点（HMM？）

* PAMI 2015 论文中的方法 GMM：每个摄像头初始化若干模式（到任意mode的概率、时间），隐变量：instance属于某个mode的概率，处于mode的时间；显变量：摄像头已经出现时间、画面中运动方向、视觉特征。好处是考虑了转移边的相似度（用模式间的转移）

  如何update？如何预测？mode间重合（unseen）？

* 二阶相似度：考虑转移边的相似度（在什么空间下讨论？）



用PAMI15的方法建立更细致的转移模型，每个摄像头出现的个体短期内有若干种转移模式（转移目标概率不同，起始时间不同，隐含的起始位置不同），先基于视觉匹配结果用GMM去fit每个个体属于模式的概率，然后进行迭代地更新。

基于转移模型带剪枝地进行 incremental 的推断。

预处理可能要用 DP/MCTS 在单摄像头内连接短片段，重新构建 id


