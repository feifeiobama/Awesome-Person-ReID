# Awesome Person ReID

This repository contains a curated list of person re-identification papers (mostly until 2021) orgnized by topics. Please feel free to pull request.

* [Survey](#Survey)
* [Supervised reID](#Supervised-reID)
  * [Pose-guided reID](##Pose-guided-reID)
  * [Attribute-guided reID](##Attribute-guided-reID)
  * [Spatial-temporal reID](##Spatial-temporal-reID)
* [Unsupervised reID](#Unsupervised-reID)
* [Generalizable reID](#Generalizable-reID)
* [Lifelong reID](#Lifelong-reID)
* [Misc topics](#Misc-topics)
  * [Cross-modality reID](##Cross-modality-reID)
  * [Long-term reID](##Long-term-reID)
  * [Group reID](##Group-reID)
  * [Person search](##Person-search)
* [Datasets](#Datasets)



## Survey

* (Book 14) Person Re-Identification
* (arXiv 16) Person Re-Identification: Past, Present and Future
* (TPAMI 18) A Systematic Evaluation and Benchmark for Person Re-Identification: Features, Metrics, and Datasets
* (TCSVT 19) A Survey of Open-World Person Re-Identification
* (IJCAI 20) Beyond Intra-Modality: A Survey of Heterogeneous Person Re-Identification
* (TPAMI 21) Deep Learning for Person Re-Identification: A Survey and Outlook
* (arXiv 22) Person Re-Identification: A Retrospective on Domain Specific Open Challenges and Future Trends



## Supervised reID

#### Global feature learning

**Verification**

* (ICPR 14) Deep Metric Learning for Person Re-Identification
* (CVPR 15) An Improved Deep Learning Architecture for Person Re-Identification
* (ECCV 16) Gated Siamese Convolutional Neural Network Architecture for Human Re-Identification
* (ICCV 17) A Two Stream Siamese Convolutional Neural Network for Person Re-Identification
* (CVPR 22) Dual Cross-Attention Learning for Fine-Grained Visual Categorization and Object Re-Identification

**Identification**

* (CVPR 16) Learning a Discriminative Null Space for Person Re-Identification
* (CVPR 17) Re-ranking Person Re-Identification with $k$-reciprocal Encoding
* (ICCV 17) SVDNet for Pedestrian Retrieval
* (arXiv 17) In Defense of the Triplet Loss for Person Re-Identification
* (TOMCCAP 17) A Discriminatively Learned CNN Embedding for Person Reidentification
* (CVPRW 19) Bag of Tricks and a Strong Baseline for Deep Person Re-Identification
* (ICCV 19) Omni-Scale Feature Learning for Person Re-Identification
* (ICCV 21) TransReID: Transformer-based Object Re-Identification
* (ACM MM 21) HAT: Hierarchical Aggregation Transformers for Person Re-identification
* (CVPR 22) NFormer: Robust Person Re-identification with Neighbor Transformer

Attention

* (CVPR 18) Harmonious Attention Network for Person Re-Identification
* (CVPR 19) Towards Rich Feature Discovery with Class Activation Maps Augmentation for Person Re-Identification
* (CVPR 19) Interaction-and-Aggregation Network for Person Re-Identification
* (ICCV 19) Mixed High-Order Attention Network for Person Re-Identification
* (ICCV 19) Second-Order Non-local Attention Networks for Person Re-Identification
* (ICCV 19) ABD-Net: Attentive but Diverse Person Re-Identification
* (CVPR 20) Relation-Aware Global Attention for Person Re-Identification

#### Local feature learning

* (CVPR 14) DeepReID: Deep Filter Pairing Neural Network for Person Re-Identification
* (ICCV 15) Person Re-Identification with Correspondence Structure Learning
* (arXiv 17) AlignedReID: Surpassing Human-Level Performance in Person Re-Identification
* (CVPR 18) End-to-End Deep Kronecker-Product Matching for Person Re-Identification
* (ECCV 18) Beyond Part Models: Person Retrieval with Refined Part Pooling (and a Strong Convolutional Baseline)
* (ACM MM 18) Learning Discriminative Features with Multiple Granularities for Person Re-Identification
* (CVPR 19) Patch-based Discriminative Feature Learning for Unsupervised Person Re-Identification
* (CVPR 21) Diverse Part Discovery: Occluded Person Re-identification with Part-Aware Transformer



### Pose-guided reID

* (CVPR 17) Spindle Net: Person Re-Identification with Human Body Region Guided Feature Decomposition and Fusion
* (ICCV 17) Deeply-Learned Part-Aligned Representations for Person Re-Identification
* (ICCV 17) Pose-driven Deep Convolutional Model for Person Re-Identification
* (CVPR 18) Pose Transferrable Person Re-Identification
* (ECCV 18) Pose-Normalized Image Generation for Person Re-Identification
* (CVPR 18) Human Semantic Parsing for Person Re-Identification
* (NeurIPS 18) FD-GAN: Pose-guided Feature Distilling GAN for Robust Person Re-Identification
* (TIP 19) Pose-Invariant Embedding for Deep Person Re-Identification
* (CVPR 19) Densely Semantically Aligned Person Re-Identification
* (ECCV 20) Identity-Guided Human Semantic Parsing for Person Re-Identification
* (ACM MM 21) Pose-guided Inter- and Intra-part Relational Transformer for Occluded Person Re-Identification
* (CVPR 22) Motion-Aware Transformer For Occluded Person Re-identification
* (TPAMI 22) Pose-Guided Representation Learning for Person Re-Identification
* (TPAMI 22) Multi-Task Learning With Coarse Priors for Robust Part-Aware Person Re-Identification
* (TNNLS 22) Parameter-Efficient Person Re-identification in the 3D Space



### Attribute-guided reID

* (ECCV 16) Deep Attributes Driven Multi-Camera Person Re-Identification
* (arXiv 17) Improving Person Re-identification by Attribute and Identity Learning
* (CVPR 18) Transferable Joint Attribute-Identity Deep Learning for Unsupervised Person Re-Identification
* (CVPR 19) AANet: Attribute Attention Network for Person Re-Identifications



### Spatial-temporal reID

* (CVPR 99) Bayesian Multi-Camera Surveillance
* (ICCV 03) Tracking across Multiple Cameras with Disjoint Views
* (CVPR 04) Bridging the Gaps between Cameras
* (CVPR 09) Multi-Camera Activity Correlation Analysis
* (ECCV 16) Human Re-Identification in Crowd Videos Using Personal, Social and Environmental Constraints
* (MMM 16) Camera Network Based Person Re-Identification by Leveraging Spatial-Temporal Constraint and Multiple Cameras Relations
* (arXiv 17) Distance-based Camera Network Topology Inference for Person Re-identification
* (ICCVW 17) Unified Framework for Automated Person Re-Identification and Camera Network Topology Inference in Camera Networks
* (CVPR 18) Unsupervised Cross-Dataset Person Re-Identification by Transfer Learning of Spatial-Temporal Patterns
* (AAAI 19) Spatial-Temporal Person Re-Identification
* (ICCV 21) Learning Instance-Level Spatial-Temporal Patterns for Person Re-Identification
* (ACM MM 21) MGH: Metadata Guided Hypergraph Modeling for Unsupervised Person Re-identification



## Unsupervised reID

#### State of the art

**Unsupervised domain adaptation  (Rank-1 Rank-5 mAP)**

| method     | reference | DukeMTMC->Market-1501 | Market-1501->DukeMTMC |
| ---------- | --------- | --------------------- | --------------------- |
| IDM        | ICCV 21   | 93.2 97.5 82.8        | 83.6 91.5 93.7        |
| GLT        | CVPR 21   | 92.2 96.5 79.5        | 82.0 90.2 69.2        |
| UNRN       | AAAI 21   | 91.9 96.1 78.1        | 82.0 90.7 69.1        |
| SpCL       | NIPS 20   | 90.3 96.2 76.7        | 82.9 90.1 68.8        |
| MEB-Net    | ECCV 20   | 89.9 96.0 76.0        | 79.6 88.3 66.1        |
| MMT        | ICLR 20   | 87.7 94.9 71.2        | 78.0 88.8 65.1        |
| CycAs      | ECCV 20   | 84.8  --:-  64.8      | 77.9  --:-  60.1      |
| AD-Cluster | CVPR 20   | 86.7 94.4 68.3        | 72.6 82.5 54.1        |
| SNR        | CVPR 20   | 82.8  --:-  61.7      | 76.3  --:-  58.1      |
| JVTC       | ECCV 20   | 83.8 93.0 61.1        | 75.0 85.1 56.2        |
| ACT        | AAAI 20   | 80.5  \-\-:\-  60.6   | 72.4  \-\-:\-  54.5   |
| MMCL       | CVPR 20   | 84.4 92.8 60.4        | 72.4 82.9 51.3        |
| SSG        | ICCV 19   | 80.0 90.0 58.3        | 73.0 80.6 53.4        |
| HCT        | CVPR 20   | 80.0 91.6 56.4        | 69.6 83.4 50.7        |
| PAST       | ICCV 19   | 78.4  \-\-:\-  54.6   | 72.4 \-\-\-:\- 54.3   |
| PDA-Net    | ICCV 19   | 75.2 86.3 47.6        | 63.2 77.0 45.1        |
| ECN        | CVPR 19   | 75.1 87.6 43.0        | 63.3 75.8 40.4        |
| PAUL       | CVPR 19   | 66.7  \-\-:\-  36.8   | 56.1  \-\-:\-  35.7   |
| CASCL      | ICCV 19   | 64.7 80.2 35.6        | 51.5 66.7 30.5        |
| SPGAN      | CVPR 18   | 58.1 76.0 26.9        | 46.9 62.6 26.4        |
| ATNet      | ICCV 19   | 55.7 73.2 25.6        | 45.1 59.5 24.9        |

Other experiment settings: MSMT17->Market-1501, MSMT17->DukeMTMC, Market-1501->MSMT17 DukeMTMC->MSMT17, CUHK03->Market-1501, CUHK03->DukeMTMC, Market-1501->PRID2011

**Unsupervised learning (Rank-1 mAP)**

| method  | reference | type        | Market1-501 | DukeMTMC         |
| ------- | --------- | ----------- | ----------- | ---------------- |
| PPLR    | CVPR 22   | clustering  | 94.3 84.4   | \-\-:\-  \-\-:\- |
| ICE     | ICCV 21   | contrastive | 93.8 82.3   | 83.3 69.9        |
| CAP     | AAAI 21   | clustering  | 91.4 79.2   | 81.1 67.3        |
| IICS    | CVPR 21   | clustering  | 89.5 72.9   | 80.0 64.4        |
| UGA     | ICCV 19   | tracklet    | 87.2 70.3   | 75.0 53.3        |
| MetaCam | CVPR 21   | clustering  | 83.9 61.7   | 73.8 53.8        |
| TAUDL   | ECCV 18   | tracklet    | 63.7 41.2   | 61.7 43.5        |
| BUC     | AAAI 19   | clustering  | 66.2 38.3   | 47.4 27.5        |

#### Organized by authors & reverse chronological

Wei-Shi Zheng (SYSU)

| proc.   | title                                                        | method                                                       | motivation                                                   |
| ------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| CVPR 20 | [Weakly supervised discriminative feature learning with state information for person identification](https://arxiv.org/pdf/2002.11939.pdf) | WDBR + DFDR: classification loss with MPI-driven decision + state sub-distribution drift regularization | state-relevant feature distortion                            |
| ICCV 19 | [Unsupervised Person Re-Identification by Camera-Aware Similarity Consistency Learning](http://openaccess.thecvf.com/content_ICCV_2019/papers/Wu_Unsupervised_Person_Re-Identification_by_Camera-Aware_Similarity_Consistency_Learning_ICCV_2019_paper.pdf) | CASCL: similarity consistency + intra-camera similarity preserving, global -> top-k neighbor | inconsistent similarity distribution (intra-camera similarity more reliable) |
| CVPR 19 | [Patch-based Discriminative Feature Learning for Unsupervised Person Re-identification](http://openaccess.thecvf.com/content_CVPR_2019/papers/Yang_Patch-Based_Discriminative_Feature_Learning_for_Unsupervised_Person_Re-Identification_CVPR_2019_paper.pdf) | PAUL: discriminative learning with patch feature bank, image-level triplet loss | the gap of similar patches is smaller than similar images    |
| CVPR 19 | [Unsupervised Person Re-identification by Soft Multilabel Learning](http://openaccess.thecvf.com/content_CVPR_2019/papers/Yu_Unsupervised_Person_Re-Identification_by_Soft_Multilabel_Learning_CVPR_2019_paper.pdf) | MAR: soft multilabel guided negative mining, similarity consistency, cross-view consistent learning | soft multilabel encodes relative comparative characteristic  |
| CVPR 19 | [Weakly Supervised Person Re-Identification](http://openaccess.thecvf.com/content_CVPR_2019/papers/Meng_Weakly_Supervised_Person_Re-Identification_CVPR_2019_paper.pdf) | CV-MIML: intra-bag alignment, cross-view bag alignment       | video-level weak label                                       |
| ICCV 17 | [Cross-view Asymmetric Metric Learning for Unsupervised Person Re-identification](http://openaccess.thecvf.com/content_ICCV_2017/papers/Yu_Cross-View_Asymmetric_Metric_ICCV_2017_paper.pdf) | CAMEL: project data into shared space, clustering            | view-specific feature distortion                             |

Yi Yang (UTS)

| proc.   | title                                                        | method                                                       | motivation                                                   |
| ------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| CVPR 19 | [Invariance Matters: Exemplar Memory for Domain Adaptive Person Re-identification](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhong_Invariance_Matters_Exemplar_Memory_for_Domain_Adaptive_Person_Re-Identification_CVPR_2019_paper.pdf) | ECN: exemplar memory for invariance learning                 | intra-domain variations, exemplar-, camera-, neighborhood-invariance |
| AAAI 19 | [A Bottom-Up Clustering Approach to Unsupervised Person Re-Identification](https://www.aaai.org/ojs/index.php/AAAI/article/view/4898) | BUC: bottom-up clustering + repelled loss training, diversity regularization | similarity and diversity in training data as supervision     |
| ECCV 18 | [Generalizing A Person Retrieval Model Hetero- and Homogeneously](http://openaccess.thecvf.com/content_ECCV_2018/papers/Zhun_Zhong_Generalizing_A_Person_ECCV_2018_paper.pdf) | HHL: camera invariance + domain correctness                  | intra- and inter- domain variance                            |
| CVPR 18 | [Exploit the Unknown Gradually: One-Shot Video-Based Person Re-Identification by Stepwise Learning](http://openaccess.thecvf.com/content_cvpr_2018/papers/Wu_Exploit_the_Unknown_CVPR_2018_paper.pdf) | EUG: select more pseudo-labeled tracklet for training during iteration, distance-based sampling criterion | initial pseudo-label predictions are unreliable              |
| CVPR 18 | [Image-Image Domain Adaptation with Preserved Self-Similarity and Domain-Dissimilarity for Person Re-identification](http://openaccess.thecvf.com/content_cvpr_2018/papers/Deng_Image-Image_Domain_Adaptation_CVPR_2018_paper.pdf) | SPGAN: contrastive loss on self-similarity and domain-dissimilarity | ID should be preserved after image translation, domains contain entirely different ID sets |
| ICCV 17 | [Unlabeled Samples Generated by GAN Improve the Person Re-identification Baseline in vitro](http://openaccess.thecvf.com/content_ICCV_2017/papers/Zheng_Unlabeled_Samples_Generated_ICCV_2017_paper.pdf) | LSRO: GAN, assign uniform label to generated data            | to use unlabeled data                                        |

Yonghong Tian (PKU)

| proc.   | title                                                        | method                                                       | motivation                           |
| ------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------ |
| ECCV 20 | [Multiple Expert Brainstorming for Domain Adaptive Person Re-identification](https://arxiv.org/pdf/2007.01546.pdf) | MEB-Net: MMT between 3 different models + ensemble based on scatter | ensemble learning remains unexplored |
| CVPR 20 | [AD-Cluster: Augmented Discriminative Clustering for Domain Adaptive Person Re-identification](https://arxiv.org/pdf/2004.08787.pdf) | generate samples with diverse camera styles                  | low diversity in cluster             |

Shiliang Zhang (PKU)

| proc.   | title                                                        | method                                                       | motivation                                          |
| ------- | ------------------------------------------------------------ | ------------------------------------------------------------ | --------------------------------------------------- |
| ECCV 20 | [Joint Visual and Temporal Consistency for Unsupervised Domain Adaptive Person Re-Identification](https://arxiv.org/pdf/2007.10854.pdf) | JVTC: local classification + global classification with temporal prob | a batch contains different id, temporal consistency |
| CVPR 20 | [Unsupervised Person Re-identification via Multi-label Classification](https://arxiv.org/pdf/2004.09228.pdf) | MMCL: multi-label + memory                                   |                                                     |

Shaogang Gong (QMUL)

| proc.   | title                                                        | method                                                       | motivation                                                   |
| ------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ECCV 18 | [Unsupervised Person Re-identification by Deep Learning Tracklet Association](http://openaccess.thecvf.com/content_ECCV_2018/papers/Minxian_Li_Unsupervised_Person_Re-identification_ECCV_2018_paper.pdf) | TAUDL: dicriminate sparse tracklets within-camera, align similar cross-camera tracklets in mini-batch | source and target domains not always share some common characteristic |
| CVPR 18 | [Transferable Joint Attribute-Identity Deep Learning for Unsupervised Person Re-Identification](http://openaccess.thecvf.com/content_cvpr_2018/papers/Wang_Transferable_Joint_Attribute-Identity_CVPR_2018_paper.pdf) | TJ-AIDL: joint learning + Identity Inferred Attribute + attribute consistency | heterogeneous attribute supervision                          |

Pong C Yuen (HKBU)

| proc.   | title                                                        | method                                                       | motivation                             |
| ------- | ------------------------------------------------------------ | ------------------------------------------------------------ | -------------------------------------- |
| ECCV 18 | [Robust Anchor Embedding for Unsupervised Video Person Re-Identification in the Wild](http://openaccess.thecvf.com/content_ECCV_2018/papers/Mang_YE_Robust_Anchor_Embedding_ECCV_2018_paper.pdf) | RACE: embedding weight of kNN anchors                        | imbalanced unlabeled data, scalability |
| ICCV 17 | [Dynamic Label Graph Matching for Unsupervised Video Re-Identification](http://openaccess.thecvf.com/content_ICCV_2017/papers/Ye_Dynamic_Label_Graph_ICCV_2017_paper.pdf) | DGM: cross-camera graph matching by neighborhood cost with re-weighed labels | cross-camera label estimation          |

**Others authors**

AAAI 21

| from | title                                                        | method                              | motivation                            |
| ---- | ------------------------------------------------------------ | ----------------------------------- | ------------------------------------- |
| USTC | [Exploiting Sample Uncertainty for Domain Adaptive Person Re-Identification](https://arxiv.org/pdf/2012.08733.pdf) | UNRN: weighted contrastive loss     | consistency between teacher & student |
| ZJU  | [Camera-aware Proxies for Unsupervised Person Re-Identification](https://arxiv.org/pdf/2012.10674.pdf) | CAP: intra-camera & inter-camera CL | camera variance                       |

ECCV 20 (3/5) (Yonghong Tian: 1, Shiliang Zhang: 1)

| from | title                                                        | method                                                       | motivation                 |
| ---- | ------------------------------------------------------------ | ------------------------------------------------------------ | -------------------------- |
| UAE  | [Interpretable and Generalizable Person Re-identification with Query-adaptive Convolution and Temporal Lifting](https://arxiv.org/pdf/1904.10424.pdf) | QAConv: query-adaptive convolutional + TLift: $\Delta T$ from pivot set | generalizablity            |
| THU  | [CycAs: Self-supervised Cycle Association for Learning Re-identifiable Descriptions](https://arxiv.org/pdf/2007.07577.pdf) | CycAs: cycle association on asymmetric pairs                 | data association in MOT    |
| CMU  | [Joint Disentangling and Adaptation for Cross-Domain Person Re-Identification](https://arxiv.org/pdf/2007.10315.pdf) | DG-Net++: DG-Net + adversarial alignment + identification loss | disentangling + adaptation |

CVPR 20 (3/6) (Wei-shi Zheng: 1, Yonghong Tian: 1, Shiliang Zhang: 1)

| from   | title                                                        | method                                                  | motivation                       |
| ------ | ------------------------------------------------------------ | ------------------------------------------------------- | -------------------------------- |
| Huawei | [Unsupervised Person Re-identification via Softened Similarity Learning](https://arxiv.org/pdf/2004.03547.pdf) | softened similarity + part + cross-camera encouragement | discard hard quantization loss   |
| USTC   | [Style Normalization and Restitution for Generalizable Person Re-identification](https://arxiv.org/pdf/2005.11037.pdf) | SNR: style normalization + distill id-relevant feature  | filter out id-irrelevant feature |
| NUDT   | [Hierarchical Clustering with Hard-batch Triplet Loss for Person Re-identification](https://arxiv.org/pdf/1910.12278.pdf) | HCT: hierarchinal  clustering + hard-batch              | pseudo label quality             |

ICLR 20 (1/1)

| from | title                                                        | method                                                       | motivation                               |
| ---- | ------------------------------------------------------------ | ------------------------------------------------------------ | ---------------------------------------- |
| CUHK | [Mutual Mean-Teaching: Pseudo Label Refinery for Unsupervised Domain Adaptation on Person Re-identification](https://openreview.net/pdf?id=rJlnOhVYPS) | MMT: optimize with soft pseudo label generated from the other network | noisy pseudo labels caused by clustering |

AAAI 20 (1/1)

| from | title                                                        | method                                                       | motivation                             |
| ---- | ------------------------------------------------------------ | ------------------------------------------------------------ | -------------------------------------- |
| XMU  | [Asymmetric Co-Teaching for Unsupervised Cross-Domain Person Re-Identification](https://arxiv.org/pdf/1912.01349.pdf) | ACT: asymetric co-teaching trained by DBSCAN labeled inliners and outliers | noisy pseudo labels, consider outliers |

ICCV 19 (5/6) (Wei-shi Zheng: 1)

| from   | title                                                        | method                                                       | motivation                                              |
| ------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------- |
| NJU    | [A Novel Unsupervised Camera-aware Domain Adaptation Framework for Person Re-identification](http://openaccess.thecvf.com/content_ICCV_2019/papers/Qi_A_Novel_Unsupervised_Camera-Aware_Domain_Adaptation_Framework_for_Person_Re-Identification_ICCV_2019_paper.pdf) | CCE: cross-domain camera equiprobability, triplet selection in fragments | camera-level subdomains, temporal continuity            |
| NTU    | [Cross-Dataset Person Re-Identification via Unsupervised Pose Disentanglement and Adaptation](http://openaccess.thecvf.com/content_ICCV_2019/papers/Li_Cross-Dataset_Person_Re-Identification_via_Unsupervised_Pose_Disentanglement_and_Adaptation_ICCV_2019_paper.pdf) | PDA-Net: pose-guided image recovery and domain translation   | jointly learn domain- and pose-invariant representation |
| UIUC   | [Self-similarity Grouping: A Simple Unsupervised Cross Domain Adaptation Approach for Person Re-identification](http://openaccess.thecvf.com/content_ICCV_2019/papers/Fu_Self-Similarity_Grouping_A_Simple_Unsupervised_Cross_Domain_Adaptation_Approach_for_ICCV_2019_paper.pdf) | SSG: 3 sets of groups, triplet loss; semi-supervised         | potential similarity from global to local               |
| Tongji | [Self-Training With Progressive Augmentation for Unsupervised Cross-Domain Person Re-Identification](http://openaccess.thecvf.com/content_ICCV_2019/papers/Zhang_Self-Training_With_Progressive_Augmentation_for_Unsupervised_Cross-Domain_Person_Re-Identification_ICCV_2019_paper.pdf) | PAST: 2-stage: CTL+RTL, global classification loss (HDBSCAN clustering, mean feature classifier) | unreliable pseudo labels, triplets focus on local info  |
| CASIA  | [Unsupervised Graph Association for Person Re-identification](http://openaccess.thecvf.com/content_ICCV_2019/papers/Wu_Unsupervised_Graph_Association_for_Person_Re-Identification_ICCV_2019_paper.pdf) | UGA: intra-camera tracklet classification, pull inter-camera pairs | underlying positive pair, lower GPU memory              |

CVPR 19 (1/5) (Wei-shi Zheng: 3, Yi Yang: 1)

| from | title                                                        | method                                                       | motivation                                     |
| ---- | ------------------------------------------------------------ | ------------------------------------------------------------ | ---------------------------------------------- |
| USTC | [Adaptive Transfer Network for Cross-Domain Person Re-Identification](http://openaccess.thecvf.com/content_CVPR_2019/papers/Liu_Adaptive_Transfer_Network_for_Cross-Domain_Person_Re-Identification_CVPR_2019_paper.pdf) | ATNet: decompose domain transfer to sub-tasks, adaptive ensemble to each image | inter-domain disparities with multiple factors |

ECCV 18 (1/4)

| from    | title                                                        | method                                     | motivation                |
| ------- | ------------------------------------------------------------ | ------------------------------------------ | ------------------------- |
| Argo AI | [Domain Adaptation through Synthesis for Unsupervised Person Re-identification](http://openaccess.thecvf.com/content_ECCV_2018/papers/Slawomir_Bak_Domain_Adaptation_through_ECCV_2018_paper.pdf) | SyRI: virtual human rendered with HDR maps | diversity in illumination |

CVPR 18 (2/5)

| from  | title                                                        | method                                  | motivation                              |
| ----- | ------------------------------------------------------------ | --------------------------------------- | --------------------------------------- |
| SCUT  | [Unsupervised Cross-dataset Person Re-identification by Transfer Learning of Spatial-Temporal Patterns](http://openaccess.thecvf.com/content_cvpr_2018/papers/Lv_Unsupervised_Cross-Dataset_Person_CVPR_2018_paper.pdf) | TFusion: bayesian fusion, learn to rank | ST indecent of feature, constant FP, FN |
| TRACE | [Disentangled Person Image Generation](http://openaccess.thecvf.com/content_cvpr_2018/papers/Ma_Disentangled_Person_Image_CVPR_2018_paper.pdf) | disentangle FG, BG, pose                | explicitly guide image genration        |

ICCV 17 (4/7)

| from  | title                                                        | method                                           | motivation                 |
| ----- | ------------------------------------------------------------ | ------------------------------------------------ | -------------------------- |
| NU    | [Efficient Online Local Metric Adaptation via Negative Samples for Person Re-Identification](http://openaccess.thecvf.com/content_ICCV_2017/papers/Zhou_Efficient_Online_Local_ICCV_2017_paper.pdf) |                                                  |                            |
| UniFI | [Group Re-Identification via Unsupervised Transfer of Sparse Features Encoding](http://openaccess.thecvf.com/content_ICCV_2017/papers/Lisanti_Group_Re-Identification_via_ICCV_2017_paper.pdf) |                                                  |                            |
| UH    | [SHaPE: A Novel Graph Theoretic Algorithm for Making Consensus-based Decisions in Person Re-identification Systems](http://openaccess.thecvf.com/content_ICCV_2017/papers/Barman_SHaPE_A_Novel_ICCV_2017_paper.pdf) | SHaPE: ranking -> shortest Hamiltonian path, ACS | aggregate multiple results |
| DUT   | [Stepwise Metric Promotion for Unsupervised Video Person Re-identification](http://openaccess.thecvf.com/content_ICCV_2017/papers/Liu_Stepwise_Metric_Promotion_ICCV_2017_paper.pdf) |                                                  |                            |

CVPR 17 (2/2)

| from            | title                                                        | method | motivation |
| --------------- | ------------------------------------------------------------ | ------ | ---------- |
| Disney Research | [One-Shot Metric Learning for Person Re-identification](http://openaccess.thecvf.com/content_cvpr_2017/papers/Bak_One-Shot_Metric_Learning_CVPR_2017_paper.pdf) |        |            |
| UCR             | [Unsupervised Adaptive Re-identification in Open World Dynamic Camera Networks](http://openaccess.thecvf.com/content_cvpr_2017/papers/Panda_Unsupervised_Adaptive_Re-Identification_CVPR_2017_paper.pdf) |        |            |



## Generalizable reID

* (CVPR 19) Generalizable Person Re-Identification by Domain-Invariant Mapping Network
* (CVPR 20) Style Normalization and Restitution for Generalizable Person Re-Identification
* (ECCV 20) Generalizing Person Re-Identification by Camera-Aware Invariance Learning and Cross-Domain Mixup
* (AAAI 21) Dual Distribution Alignment Network for Generalizable Person Re-Identification
* (CVPR 21) Meta Batch-Instance Normalization for Generalizable Person Re-Identification
* (CVPR 21) Generalizable Person Re-Identification with Relevance-aware Mixture of Experts



## Lifelong reID

* (AVSS 19) Continuous Learning without Forgetting for Person Re-Identification
* (AAAI 21) Generalising without Forgetting for Lifelong Person Re-Identification
* (WACV 21) Continual Representation Learning for Biometric Identification
* (CVPR 21) Lifelong Person Re-Identification via Adaptive Knowledge Accumulation
* (AAAI 22) Lifelong Person Re-identification by Pseudo Task Knowledge Preservation
* (CVPR 22) Lifelong Unsupervised Domain Adaptive Person Re-Identification with Coordinated Anti-forgetting and Adaptation
* (ACM MM 22) Patch-based Knowledge Distillation for Lifelong Person Re-Identification
* (ACM MM 22) Meta Reconciliation Normalization for Lifelong Person Re-Identification



## Misc topics

### Cross-modality reID

* (ICCV 17) RGB-Infrared Cross-Modality Person Re-Identification
* (IJCAI 18) Cross-Modality Person Re-Identification with Generative Adversarial Training
* (CVPR 19) Learning to Reduce Dual-Level Discrepancy for Infrared-Visible Person Re-Identification
* (ICCV 19) RGB-Infrared Cross-Modality Person Re-Identification via Joint Pixel and Feature Alignment
* (AAAI 20) Cross-Modality Paired-Images Generation for RGB-Infrared Person Re-Identification
* (CVPR 20) Hi-CMD: Hierarchical Cross-Modality Disentanglement for Visible-Infrared Person Re-Identification
* (CVPR 20) Cross-Modality Person Re-Identification with Shared-Specific Feature Transfer
* (ECCV 20) Dynamic Dual-Attentive Aggregation Learning for Visible-Infrared Person Re-Identification
* (CVPR 21) Neural Feature Search for RGB-Infrared Person Re-Identification
* (CVPR 21) Farewell to Mutual Information: Variational Distillation for Cross-Modal Person Re-Identification
* (CVPR 21) Discover Cross-Modality Nuances for Visible-Infrared Person Re-Identification
* (ICCV 21) Syncretic Modality Collaborative Learning for Visible Infrared Person Re-Identification
* (ICCV 21) Learning by Aligning: Visible-Infrared Person Re-Identification Using Cross-Modal Correspondences
* (ICCV 21) Cross-Modality Person Re-Identification via Modality Confusion and Center Aggregation

#### State of the art

* SYSU-MM01: MCLNet
* RegDB: SMCL



###Long-term reID

* (TPAMI 19) Person Re-Identification by Contour Sketch under Moderate Clothing Change
* (IJCNN 19) Celebrities-ReID: A Benchmark for Clothes Variation in Long-Term Person Re-Identification
* (ACCV 20) Long-Term Cloth-Changing Person Re-Identification
* (CVPR 20) COCAS: A Large-Scale Clothes Changing Person Dataset for Re-Identification



### Group reID

* (BMVC 09) Associating Groups of People
* (ICCV 17) Group Re-Identification via Unsupervised Transfer of Sparse Features Encoding
* (ACM MM 18) Group Re-Identification: Leveraging and Integrating Multi-Grain Information
* (CVPR 19) Learning Context Graph for Person Search
* (CVPR 22) Modeling 3D Layout for Group Re-Identification

#### Reading notes

Duke: DukeMTMC group dataset, Road: Road group dataset

| from  | method                                                       | motivation                                   | Duke rank1 | Duke rank5 | Road rank1 | Road rank5 |
| ----- | ------------------------------------------------------------ | -------------------------------------------- | ---------- | ---------- | ---------- | ---------- |
| QMUL  | (BMVC 09) CRRRO-BRO: 2 descriptors of ring regions           | rotation invariant                           | 9.9        | 26.1       | 17.8       | 34.6       |
| OYO   | (ICPR 10) covariance descriptor                              | illumination invariance                      | 21.3       | 43.6       | 38.9       | 61.0       |
| USTC  | (ICIP 16) BSC+CM: salience channel +consistent matching      | unreliable patch matches                     | 23.1       | 44.3       | 58.6       | 80.6       |
| UniFI | (ICCV 17) PREF: mask + sparse encoding                       | spatial displacement                         | 22.3       | 44.3       | 43.0       | 68.7       |
| SJTU  | (MM 18) MGR: multi-grain representation + matching           | group granularity                            | 47.4       | 68.1       | 72.3       | 90.6       |
| SJTU  | (TCYB 19) hand=>conv                                         | utilize dl                                   | 48.4       | 75.2       | 80.2       | 93.8       |
| NTHU  | (arXiv 19) DotSCN: learn single&couple representation on transferred reID dataset | too few images to learn group representation | 86.4       | 98.8       | 84.0       | 95.1       |



### Person search

* (ACM MM 14) Person Search in a Scene by Jointly Modeling People Commonness and Person Uniqueness
* (CVPR 17) Joint Detection and Identification Feature Learning for Person Search
* (ICCV 17) Neural Person Search Machines
* (ICCV 19) Re-ID Driven Localization Refinement for Person Search
* (CVPR 20) Robust Partial Matching for Person Search in the Wild
* (CVPR 20) Norm-Aware Embedding for Efficient Person Search
* (CVPR 21) Anchor-Free Person Search

#### Reading notes


| from  | method                                               | motivation                    | mAP (CUHK-SYSU) | top-1 (CUHK-SYSU) | mAP (PRW) | top-1 (PRW) |
| ----- | ---------------------------------------------------- | ----------------------------- | --------------- | ----------------- | --------- | ----------- |
| CUHK  | (CVPR 17) OIM: online matching with lookup table     | joint detection and reID      | 75.5            | 78.7              | 21.3      | 49.9        |
| TUM   |                                                      | => larger image               | 83.3            | 84.2              | 38.3      | 70.0        |
| XJTU  | (arXiv 2017) IAN: center loss                        | intra-class variance          | 77.2            | 80.5              | 23.0      | 61.9        |
| HFUT  | (ICCV 17) NPSM: recursive region shrinking with lstm | query-guided proposal         | 77.9            | 81.2              | 24.2      | 53.0        |
| CMU   | (ECCV 18) RCAA: context-aware agent modifies bbox    | query-guided proposal with RL | 79.5            | 81.3              | -         | -           |
| NJUST | (ECCV 18) MGTS: mask-guided two-stream               | emphasize foreground info     | 83.0            | 83.7              | 32.6      | 72.1        |
| QMUL  | (ECCV 18) CLSA: in-network feature pyramid           | multi-scale feature           | 87.2            | 88.5              | 38.7      | 65.0        |
| SJTU  | (CVPR 19) contextual instance graph                  | learn contexual info          | 84.1            | 86.5              | 33.4      | 73.6        |
| TUM   | (CVPR 19) QEEPS: query-guided SSE-Net, RPN, simNet   | leverage query extensively    | 88.9            | 89.1              | 39.1      | 80.0        |
| HUST  | (ICCV 19) regression => reID gradient                | refine detection              | 93.0            | 94.2              | 42.9      | 70.2        |

person search = detection + re-identification



## Datasets

| Dataset       | from   | time | description             | # identities | # cameras   | # images |
| ------------- | ------ | ---- | ----------------------- | ------------ | ----------- | -------- |
| VIPeR         | UCSC   | 2007 | -                       | 632          | 2           | 1264     |
| QMUL iLIDS    | QMUL   | 2009 | airport                 | 119          | 2           | 476      |
| GRID          | QMUL   | 2009 | underground             | 1025         | 8           | 1275     |
| PRID2011      | TUGraz | 2011 | campus                  | 934          | 2           | 24541    |
| CUHK01        | CUHK   | 2012 | campus                  | 971          | 2           | 3884     |
| CUHK02        | CUHK   | 2013 | campus                  | 1816         | 10(5 pairs) | 7264     |
| CUHK03        | CUHK   | 2014 | campus                  | 1467         | 10(5 pairs) | 13164    |
| iLIDS-VID     | QMUL   | 2014 | iLIDS video             | 300          | 2           | 42495    |
| Market1501    | THU    | 2015 | campus supermarket      | 1501         | 6           | 32217    |
| PKU-Reid      | PKU    | 2016 | 8 orientations          | 114          | 2           | 1824     |
| PRW           | UTS    | 2016 | Market1501 full frame   | 932          | 6           | 34304    |
| MARS          | THU    | 2016 | Market1501 video        | 1261         | 6           | 1191003  |
| DukeMTMC-reID | Duke   | 2017 | campus                  | 1812         | 8           | 36441    |
| DukeMTMC4RID  | Duke   | 2017 | Duke SOTA detector      | 1852         | 8           | 46261    |
| MSMT17        | PKU    | 2018 | scene & lighting change | 4101         | 15          | 126441   |

