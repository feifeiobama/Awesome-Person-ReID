## Spatial-temporal re-id notes

| from | method                                                       | motivation                                   | full name | D rank1 | D mAP | M rank1 | M mAP |
| ---- | ------------------------------------------------------------ | -------------------------------------------- | --------- | ------- | ----- | ------- | ----- |
| UCF  | (ECCV 16) [PSE](https://link.springer.com/chapter/10.1007/978-3-319-46475-6_8): speed, grouping, invisible speed | corwds & social force                        |           |         |       |         |       |
| WHU  | (MMM 16) [CNPR](https://link.springer.com/chapter/10.1007/978-3-319-27671-7_15): fit Weibull distribution | constraints of min walking time              |           |         |       |         |       |
| GIST | (17) distance based camera network topology inference        | infer topology, deal with speed              |           |         |       |         |       |
| GIST | (ICCV 17 Workshop) [unified](https://arxiv.org/abs/1704.07085): R-squared statics; cam2cam & zone2zone | solve ... jointly                            |           |         |       |         |       |
| SCUT | (CVPR 18) [TFusion](https://arxiv.org/abs/1803.07293): bayesian fusion; learn to rank | similarity, FP, FT are independent of camera |           |         |       | 73.1    |       |
| SYSU | (AAAI 19) [st-ReID](https://arxiv.org/abs/1812.03282): laplace smoothing + logistic | joint metric                                 |           | 94.4    | 83.9  | 98.1    | 87.6  |
|      | st-ReID + k-reciprocal                                       |                                              |           | 94.5    | 92.7  | 98.0    | 95.5  |
| USTC | [TASTR](https://arxiv.org/abs/1910.11560): within-/cross-camera triplet loss | precision of tracklet association            |           | 74.1    | 54.4  |         |       |

D: DukeMTMC, M: Market-1501

