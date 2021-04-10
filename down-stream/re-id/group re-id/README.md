## Group re-id notes

Duke: DukeMTMC group dataset, Road: Road group dataset

| from     | method                                                       | motivation                                       | Duke rank1 | Duke rank5 | Road rank1 | Road rank5 |
| -------- | ------------------------------------------------------------ | ------------------------------------------------ | ---------- | ---------- | ---------- | ---------- |
| QMUL     | (BMVC 09) CRRRO-BRO: 2 descriptors of ring regions           | rotation invariant                               | 9.9        | 26.1       | 17.8       | 34.6       |
| OYO      | (ICPR 10) covariance descriptor                              | illumination invariance                          | 21.3       | 43.6       | 38.9       | 61.0       |
| USTC     | (ICIP 16) BSC+CM: salience channel +consistent matching      | unreliable patch matches                         | 23.1       | 44.3       | 58.6       | 80.6       |
| UniFI    | (ICCV 17) PREF: mask + sparse encoding                       | spatial displacement                             | 22.3       | 44.3       | 43.0       | 68.7       |
| **SJTU** | **(MM 18) MGR: multi-grain representation + matching**       | **group granularity**                            | **47.4**   | **68.1**   | **72.3**   | **90.6**   |
| SJTU     | (TCYB 19) hand=>conv                                         | utilize dl                                       | 48.4       | 75.2       | 80.2       | 93.8       |
| **NTHU** | **TSCN: learn single&couple representation on transferred reID dataset** | **too few images to learn group representation** | **86.4**   | **98.8**   | **84.0**   | **95.1**   |



PREF 及之前的工作：(1) 设计descriptor (2) 当作patch matching任务

MGR 与 TSCN 比较（唯二基于检测个体的工作）

|      | group similarity                                 | geometry信息   |
| ---- | ------------------------------------------------ | -------------- |
| MGR  | 基于single similarity和距离，自下而上计算4项融合 | 利用图片中距离 |
| TSCN | 融合single similarity和另学的couple similarity   | 完全丢弃       |
