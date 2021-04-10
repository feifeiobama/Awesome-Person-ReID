## Notes on Temporal Action Localization

### A. Unsupervised

#### 1. Unsupervised Human Action Detection by Action Matching

###### CVPR 2017 Workshops. The Australian National University; Queensland University of Technology

Fused features (HOG+HOF+MBF) -> Smoothing -> Normalize -> <u>Rank Pooling</u> -> Candidate generation (temporal consistency)

F1 score: MPII cooking: 15.1%; IKEA: 25.1%; THUMOS15: 19.5%

#### 2. Unsupervised Action Discovery and Localization in Videos

###### ICCV 2017. Center for Research in Computer Vision (CRCV); University of Central Florida (UCF)

1. Action Discovery through Discriminative Clustering

   dominant set, <u>replicator dynamics</u> (SVM, select top)

2. Spatio-temporal Annotation using Knapsack

   supervoxels -> Knapsack (value, weight, temporal constraint)

AUC of ROC: UCF Sports; JHMDB; sub-JHMDB; THUMOS13; UCF101 (= state-of-art supervised method)

### B. Weakly-supervised

#### 1. UntrimmedNets for Weakly Supervised Action Recognition and Detection

###### CVPR 2017. ETH Zurich; The Chinese University of Hong Kong

> previous weakly supervised
>
> * movie script: aligned
> * an ordered list of action classes: order info

End-to-end: clip (shot-based sampling: HOG) -> <u>UntrimmedNet</u>: feature (two-stream: spatial, temporal), classification, selection (hard: MIL * soft: attention) prediction (without spatial)

WSR, WSD: HMDB51, UCF101; THUMOS14 (IoU threshold=0.5 detection 13.7%), ActivityNet (>= strongly supervised approaches)

#### 2. Hide-and-Seek: Forcing a Network to be Meticulous for Weakly-supervised Object and Action Localization

###### ICCV 2017. University of California, DavisTrain: Step-by-step Erasion.

object localization (ILSVRC dataset) & action localization

dropout => bias; max pooling > avg pooling

<u>hide frames</u> -> activation maps (THUMOS IoU=0.5 6.11->6.84)

#### 3. Weakly Supervised Action Localization by Sparse Temporal Pooling Network

###### CVPR 2018. University of California, Irvine; Google; Seoul National University

video-level class labels -> temporal intervals of human action (no localization annotation)

two-stream (RGB, optical) -> I3D -> uniformly sample segmentaion -> action classification (attention)

-> temporal class activation map -> localization

THUMOS14; ActivityNet1.3 (validation IoU=0.5: AP=29.3; test mAP=20.07)

#### 4. Step-by-step Erasion, One-by-one Collection: A Weakly Supervised Temporal Action Detector 21.2%

###### ACM Mutimedia 2018. Peking University

classifier -> detector

* Train: Step-by-step Erasion. snippet -> erasing probability -> repeat
* Test: One-by-one Collection.

#### 5. AutoLoc: Weakly-supervised Temporal Action Localization in Untrimmed Videos

###### ECCV 2018. Columbia University; Microsoft Research; Mitsubishi Electric

TAL, temporal boundary

Outer-Inner-Contrastive loss, Class Activation Sequence (CAS)

generic boundary predictor

mAP (IoU threshold=0.5) THUMOS14 13.7%-> 21.2%; ActivityNet 7.4% -> 27.3%