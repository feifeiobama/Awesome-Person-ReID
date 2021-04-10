## Hough transform notes

#### Hough forests

training -> probablistic vote

regress the displacement vector to reference point & object class

> (CVPR 09) [Class-Specific Hough Forests for Object Detection](https://pages.iai.uni-bonn.de/gall_juergen/download/jgall_houghforest_cvpr09.pdf)
>
> (CVPR 10) [A Hough Transform-Based Voting Framework for Action Recognition](http://www.vision.ee.ethz.ch/~yaoa/pdfs/yao_gall_vgool_cvpr2010.pdf)
>
> (TPAMI 11) [Hough Forests for Object Detection, Tracking, and Action Recognition](http://www.ipb.uni-bonn.de/html/projects/MoD/literatur/pdf/p7-2011_Gall_Houghforests.pdf)

#### VoteNet

end2end train: sampling (PointNet) -> voting -> clustering -> proposal (PointNet)

supervision of center, heading angle, box size, semantic classification

> (ICCV 19) [Deep Hough Voting for 3D Object Detection in Point Clouds](http://openaccess.thecvf.com/content_ICCV_2019/papers/Qi_Deep_Hough_Voting_for_3D_Object_Detection_in_Point_Clouds_ICCV_2019_paper.pdf)

#### Survey

Standard HT: accumulate all parameter $a$ such that $f(x,a)=0$

Generalized HT: construct R-table to reference point

Randomized HT:  many to one mapping

> [A survey of Hough Transform](https://www.sciencedirect.com/science/article/abs/pii/S0031320314003446)
>
> [Generalizing the hough transform to detect arbitrary shapes](https://www.cs.bgu.ac.il/~icbv161/wiki.files/Readings/1981-Ballard-Generalizing_the_Hough_Transform_to_Detect_Arbitrary_Shapes.pdf)