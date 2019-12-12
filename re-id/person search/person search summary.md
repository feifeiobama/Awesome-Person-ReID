| from  | method                                               | motivation                    | mAP (CUHK-SYSU) | top-1 (CUHK-SYSU) | mAP (PRW) | top-1 (PRW) |
| ----- | ---------------------------------------------------- | ----------------------------- | --------------- | ----------------- | --------- | ----------- |
| CUHK  | (CVPR 17) OIM: online matching with lookup table     | joint detection and reID      | 75.5            | 78.7              | 21.3      | 49.9        |
| TUM   |                                                      | => larger image               | 83.3            | 84.2              | 38.3      | 70.0        |
| XJTU  | (2017) IAN: center loss                              | intra-class variance          | 77.2            | 80.5              | 23.0      | 61.9        |
| HFUT  | (ICCV 17) NPSM: recursive region shrinking with lstm | query-guided proposal         | 77.9            | 81.2              | 24.2      | 53.0        |
| CMU   | (ECCV 18) RCAA: context-aware agent modifies bbox    | query-guided proposal with RL | 79.5            | 81.3              | -         | -           |
| NJUST | (ECCV 18) MGTS: mask-guided two-stream               | emphasize foreground info     | 83.0            | 83.7              | 32.6      | 72.1        |
| QMUL  | (ECCV 18) CLSA: in-network feature pyramid           | multi-scale feature           | 87.2            | 88.5              | 38.7      | 65.0        |
| SJTU  | (CVPR 19) contextual instance graph                  | learn contexual info          | 84.1            | 86.5              | 33.4      | 73.6        |
| TUM   | (CVPR 19) QEEPS: query-guided SSE-Net, RPN, simNet   | leverage query extensively    | 88.9            | 89.1              | 39.1      | 80.0        |
| HUST  | (ICCV 19) regression => reID gradient                | refine detection              | 93.0            | 94.2              | 42.9      | 70.2        |



person search = detection + re-identification，大部分工作改进其中一部分，或都改进