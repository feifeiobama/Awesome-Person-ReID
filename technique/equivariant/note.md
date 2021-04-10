##### AET系列工作

AET (CVPR'19)

* $l(t,t')=\begin{cases}\frac{1}{2}\|M(\theta)-M(\theta')\|^2&t_\theta\\\frac{1}{2}\|z-z'\|^2&t_z(x)=G(x,z)\\E_{x\sim\mathcal{X}}\text{dist}(t(x),t'(x))&\text{non-parametric}\end{cases}$
* arranging transformation: AET-projective

AETv2

* Euclidean distance -> geodesic distance

AVT (ICCV'19)

* maximize variational lower bound of $I(t;z|\tilde z)$

EnAET (TIP'20)

* spatial: projective, affine, similarity, euclidean
* non-spatial: color, contrast, brightness, sharpness

GraphTER (CVPR'20)

* node-wise graph signal transformation
* EdgeConv

TrGAN (CVPR'20)

* internal feature matching within E & G
* feature transformation matching for generated $h_i$

equivariant相比invariant的优势

* 无需大量data
* 生成变换比生成data的自由度低



##### Equivariant相关工作

Steerable filter (TPAMI'91)

* adaptively steer a filter to any orientation 

Capsule (ICANN'11)

* probability invariant
* viewpoint equivariant

Group equivariant CNN (ICML'16)

* 



##### 应用到re-ID

是否集成id&transform, invariance&equivariance?

可用transform
* sptial: translation, scale
* ~~style: color, contrast, brightness, sharpness~~ 结构更重要
* ~~structure: pose, viewpoint~~ 生成较难
* content: background, occlusion, random patch/erase

有意义的transform
* 传统：裁剪、抹去
* 局部比例：把腿p长，把人p瘦

