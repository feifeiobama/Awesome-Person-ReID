## Camera topology notes

| from   | title                                                        | method                                                       |
| ------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| CU     | (CVPR 99) Bayesian Multi-camera Surveillance                 | posterior decomposed into incident chains, MAP->LP           |
| KUL    | (CVPR 04) Bridging the Gaps between Cameras                  | cross correlation between zones (classified by GMM)          |
| McGill | (CRV 05) Topology inference for a vision-based sensor network | use MCEM to solve connectivity                               |
| MIT    | (ICCV 05) Inference of Non-Overlapping Camera Network Topology by Measuring Statistical Dependence | MAP approximation for MI with MCMC                           |
| CUHK   | (TPAMI 08) Correspondence-Free Activity Analysis and Scene Modeling in Multiple Camera Views | cluster trajectory according to assigned activities          |
| QMUL   | (CVPR 09) Multi-Camera Activity Correlation Analysis         | activity correlation between regions (clustered by decomposition) |
| NTU    | (TMM 11) Adaptive Learning for Target Tracking and True Linking Discovering Across Multiple Non-Overlapping Cameras | GMM with merge/split, remove weak links                      |
| GIST   | (PRL 17) Distance-based Camera Network Topology Inference for Person Re-identification | scale & speed & distance estimation                          |
| GIST   | (ICCV 17 Workshop) Unified Framework for Automated Person Re-identification and Camera Network Topology Inference in Camera Networks | connectivity check via gaussian model                        |

