## State of the art

#### Adaption methods  (Rank-1 Rank-5 mAP)

| method | reference | DukeMTMC->Market1-501 | Market-1501->DukeMTMC |
| --------- | -------------- | --------- | --------- |
| SSG      | ICCV 19 | 86.2 94.6 68.7 | 76.0 85.8 60.3 |
| PAST | ICCV 19 | 78.4  \-\-:\-  54.6 | 72.4 \-\-\-:\- 54.3 |
| PDA-Net | ICCV 19 | 75.2 86.3 47.6 | 63.2 77.0 45.1 |
| ECN | CVPR 19 | 75.1 87.6 43.0 | 63.3 75.8 40.4 |
| PAUL | CVPR 19 | 66.7  \-\-:\-  36.8 | 56.1  \-\-:\-  35.7 |
| CASCL     | ICCV 19 | 64.7 80.2 35.6 | 51.5 66.7 30.5 |
| SPGAN | CVPR 18 | 58.1 76.0 26.9 | 46.9 62.6 26.4 |
| ATNet | ICCV 19 | 55.7 73.2 25.6 | 45.1 59.5 24.9 |

Other experiment settings: MSMT17->Market-1501, MSMT17->DukeMTMC, Market-1501->**MSMT17** DukeMTMC->**MSMT17**, CUHK03->Market-1501, CUHK03->DukeMTMC, Market-1501->**PRID2011** (**bold** means difficult)

#### Methods without source domain pretrain (Rank-1 mAP)

| method | reference | type | Market1-501 | DukeMTMC |
| --------- | -------------- | -------------- | --------- | --------- |
| UGA | ICCV 19 | tracklet | 87.2 70.3 | 75.0 53.3 |
| TAUDL  | ECCV 18   | tracklet | 63.7 41.2   | 61.7 43.5 |
| BUC    | AAAI 19   | cluster  | 66.2 38.3   | 47.4 27.5 |

## Sort by author

Wei-Shi Zheng (SYSU)

| proc.   | title                                                        | method                                                       | motivation                                                   |
| ------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ICCV 19 | [Unsupervised Person Re-Identification by Camera-Aware Similarity Consistency Learning](http://openaccess.thecvf.com/content_ICCV_2019/papers/Wu_Unsupervised_Person_Re-Identification_by_Camera-Aware_Similarity_Consistency_Learning_ICCV_2019_paper.pdf) | CASCL: similarity consistency + intra-camera similarity preserving, global -> top-k neighbor | inconsistent similarity distribution (intra-camera similarity more reliable) |
| CVPR 19 | [Patch-based Discriminative Feature Learning for Unsupervised Person Re-identification](http://openaccess.thecvf.com/content_CVPR_2019/papers/Yang_Patch-Based_Discriminative_Feature_Learning_for_Unsupervised_Person_Re-Identification_CVPR_2019_paper.pdf) | PAUL: discriminative learning with patch feature bank, image-level triplet loss | the gap of similar patches is smaller than similar images    |
| CVPR 19 | [Unsupervised Person Re-identification by Soft Multilabel Learning](http://openaccess.thecvf.com/content_CVPR_2019/papers/Yu_Unsupervised_Person_Re-Identification_by_Soft_Multilabel_Learning_CVPR_2019_paper.pdf) | MAR: soft multilabel guided negative mining, similarity consistency, cross-view consistent learning | soft multilabel encodes relative comparative characteristic  |
| CVPR 19 | [Weakly Supervised Person Re-Identification](http://openaccess.thecvf.com/content_CVPR_2019/papers/Meng_Weakly_Supervised_Person_Re-Identification_CVPR_2019_paper.pdf) |                                                              |                                                              |
| ICCV 17 | [Cross-view Asymmetric Metric Learning for Unsupervised Person Re-identification](http://openaccess.thecvf.com/content_ICCV_2017/papers/Yu_Cross-View_Asymmetric_Metric_ICCV_2017_paper.pdf) | CAMEL: project data into shared space, clustering            | view-specific feature distortion                             |

Yi Yang (UTS)

| proc.   | title                                                        | method                                                       | motivation                                                   |
| ------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| CVPR 19 | [Invariance Matters: Exemplar Memory for Domain Adaptive Person Re-identification](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhong_Invariance_Matters_Exemplar_Memory_for_Domain_Adaptive_Person_Re-Identification_CVPR_2019_paper.pdf) | ECN: exemplar memory for invariance learning                 | intra-domain variations, exemplar-, camera-, neighborhood-invariance |
| AAAI 19 | [A Bottom-Up Clustering Approach to Unsupervised Person Re-Identification](https://www.aaai.org/ojs/index.php/AAAI/article/view/4898) | BUC: bottom-up clustering + repelled loss training, diversity regularization | similarity and diversity in training data as supervision     |
| ECCV 18 | [Generalizing A Person Retrieval Model Hetero- and Homogeneously](http://openaccess.thecvf.com/content_ECCV_2018/papers/Zhun_Zhong_Generalizing_A_Person_ECCV_2018_paper.pdf) |                                                              |                                                              |
| CVPR 18 | [Exploit the Unknown Gradually: One-Shot Video-Based Person Re-Identification by Stepwise Learning](http://openaccess.thecvf.com/content_cvpr_2018/papers/Wu_Exploit_the_Unknown_CVPR_2018_paper.pdf) | EUG: select more pseudo-labeled tracklet for training during iteration, distance-based sampling criterion | initial pseudo-label predictions are unreliable              |
| CVPR 18 | [Image-Image Domain Adaptation with Preserved Self-Similarity and Domain-Dissimilarity for Person Re-identification](http://openaccess.thecvf.com/content_cvpr_2018/papers/Deng_Image-Image_Domain_Adaptation_CVPR_2018_paper.pdf) | SPGAN: contrastive loss on self-similarity and domain-dissimilarity | ID should be preserved after image translation, domains contain entirely different ID sets |
| ICCV 17 | [Unlabeled Samples Generated by GAN Improve the Person Re-identification Baseline in vitro](http://openaccess.thecvf.com/content_ICCV_2017/papers/Zheng_Unlabeled_Samples_Generated_ICCV_2017_paper.pdf) | LSRO: GAN, assign uniform label to generated data            | to use unlabeled data                                        |

Shaogang Gong (QMUL)

| proc.   | title                                                        | method                                                       | motivation                                                   |
| ------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ECCV 18 | [Unsupervised Person Re-identification by Deep Learning Tracklet Association](http://openaccess.thecvf.com/content_ECCV_2018/papers/Minxian_Li_Unsupervised_Person_Re-identification_ECCV_2018_paper.pdf) | TAUDL: dicriminate sparse tracklets within-camera, align similar cross-camera tracklets in mini-batch | source and target domains not always share some common characteristic |
| CVPR 18 | [Transferable Joint Attribute-Identity Deep Learning for Unsupervised Person Re-Identification](http://openaccess.thecvf.com/content_cvpr_2018/papers/Wang_Transferable_Joint_Attribute-Identity_CVPR_2018_paper.pdf) | TJ-AIDL:                                                     |                                                              |

Pong C Yuen (HKBU)

| proc.   | title                                                        | method                                | motivation                             |
| ------- | ------------------------------------------------------------ | ------------------------------------- | -------------------------------------- |
| ECCV 18 | [Robust Anchor Embedding for Unsupervised Video Person Re-Identification in the Wild](http://openaccess.thecvf.com/content_ECCV_2018/papers/Mang_YE_Robust_Anchor_Embedding_ECCV_2018_paper.pdf) | RACE: embedding weight of kNN anchors | imbalanced unlabeled data, scalability |
| ICCV 17 | [Dynamic Label Graph Matching for Unsupervised Video Re-Identification](http://openaccess.thecvf.com/content_ICCV_2017/papers/Ye_Dynamic_Label_Graph_ICCV_2017_paper.pdf) |                                       |                                        |

#### Others authors

ICCV 19 (5/6) (Wei-shi Zheng: 1)

| from   | title                                                        | method                                                       | motivation                                                   |
| ------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| NJU    | [A Novel Unsupervised Camera-aware Domain Adaptation Framework for Person Re-identification](http://openaccess.thecvf.com/content_ICCV_2019/papers/Qi_A_Novel_Unsupervised_Camera-Aware_Domain_Adaptation_Framework_for_Person_Re-Identification_ICCV_2019_paper.pdf) | CCE:                                                         |                                                              |
| NTU    | [Cross-Dataset Person Re-Identification via Unsupervised Pose Disentanglement and Adaptation](http://openaccess.thecvf.com/content_ICCV_2019/papers/Li_Cross-Dataset_Person_Re-Identification_via_Unsupervised_Pose_Disentanglement_and_Adaptation_ICCV_2019_paper.pdf) | PDA-Net: pose-guided image recovery and domain translation   | jointly learn domain- and pose-invariant representation      |
| UIUC   | [Self-similarity Grouping: A Simple Unsupervised Cross Domain Adaptation Approach for Person Re-identification](http://openaccess.thecvf.com/content_ICCV_2019/papers/Fu_Self-Similarity_Grouping_A_Simple_Unsupervised_Cross_Domain_Adaptation_Approach_for_ICCV_2019_paper.pdf) | SSG: assign pseudo label for 3 sets of groups, triplet loss  | potential similarity from global to local                    |
| Tongji | [Self-Training With Progressive Augmentation for Unsupervised Cross-Domain Person Re-Identification](http://openaccess.thecvf.com/content_ICCV_2019/papers/Zhang_Self-Training_With_Progressive_Augmentation_for_Unsupervised_Cross-Domain_Person_Re-Identification_ICCV_2019_paper.pdf) | PAST: 2-stage: ranking-based triplet loss, softmax cross-entropy loss | unreliable pseudo labels, triplets focus on local info       |
| CASIA  | [Unsupervised Graph Association for Person Re-identification](http://openaccess.thecvf.com/content_ICCV_2019/papers/Wu_Unsupervised_Graph_Association_for_Person_Re-Identification_ICCV_2019_paper.pdf) | UGA:                                                         | TAUDL need large batch size, RACE / BUC sensitive to noisy pairs |

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
| TRACE | [Disentangled Person Image Generation](http://openaccess.thecvf.com/content_cvpr_2018/papers/Ma_Disentangled_Person_Image_CVPR_2018_paper.pdf)                         | disentangle FG, BG, pose                | explicitly guide image genration        |

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
| Disney Research | [One-Shot Metric Learning for Person Re-identification](http://openaccess.thecvf.com/content_cvpr_2017/papers/Bak_One-Shot_Metric_Learning_CVPR_2017_paper.pdf)        |        |            |
| UCR             | [Unsupervised Adaptive Re-identification in Open World Dynamic Camera Networks](http://openaccess.thecvf.com/content_cvpr_2017/papers/Panda_Unsupervised_Adaptive_Re-Identification_CVPR_2017_paper.pdf) |        |            |