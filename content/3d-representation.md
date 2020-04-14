# Learning 3D Representations From Natural Images

This repository is a collection of papers on learning 3D representations from natural images.

## Table of Contents
- [3D Shape Representation and Feature Embedding](#3d-shape-representation-and-feature-embedding)
- [Representation of Motion](#representation-of-motion)
- [Surface Cuts and Parameterization](#surface-cuts-and-parameterization)
- [Dense Shape Correspondence & Matching](#dense-shape-correspondence---matching)
- [3D Reconstruction with Synthesied Images](#3d-reconstruction-with-synthesied-images)

## 3D Shape Representation and Feature Embedding

**LIMP: Learning Latent Shape Representations with Metric Preservation Priors.**<br>
*Luca Cosmo, Antonio Norelli, Oshri Halimi, Ron Kimmel, Emanuele Rodolà.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2003.12283)]

**Learning 3D Part Assembly from a Single Image.**<br>
*Yichen Li, Kaichun Mo, Lin Shao, Minhyuk Sung, Leonidas Guibas.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2003.09754)]

**Curriculum DeepSDF.**<br>
*Yueqi Duan, Haidong Zhu, He Wang, Li Yi, Ram Nevatia, Leonidas J. Guibas.*<br>
arxiv, 19 Mar 2020. [[PDF](https://arxiv.org/abs/2003.08593)] [[Github](https://github.com/haidongz-usc/Curriculum-DeepSDF)]

**NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis.**<br>
*[Ben Mildenhall](http://people.eecs.berkeley.edu/~bmild/), [Pratul P. Srinivasan](https://people.eecs.berkeley.edu/~pratul/), [Matthew Tancik](http://www.matthewtancik.com/), [Jonathan T. Barron](https://jonbarron.info/), [Ravi Ramamoorthi](http://cseweb.ucsd.edu/~ravir/), [Ren Ng](https://www2.eecs.berkeley.edu/Faculty/Homepages/yirenng.html).*<br>
arxiv, 19 Mar 2020. [[PDF](https://arxiv.org/abs/2003.08934)] [[Project](http://tancik.com/nerf)] [[Gtihub-Tensorflow](https://github.com/bmild/nerf)] [[krrish94-PyTorch](https://github.com/krrish94/nerf-pytorch)] [[yenchenlin-PyTorch](https://github.com/yenchenlin/nerf-pytorch)]

**PolyGen: An Autoregressive Generative Model of 3D Meshes.**<br>
*Charlie Nash, Yaroslav Ganin, S. M. Ali Eslami, Peter W. Battaglia.*<br>
arxiv, 23 Feb 2020. [[PDF](https://arxiv.org/abs/2002.10880)]

**Self-supervised Learning of 3D Objects from Natural Images.**<br>
*Hiroharu Kato, Tatsuya Harada.*<br>
arxiv, 20 Nov. 2019. [[PDF](https://arxiv.org/abs/1911.08850)] [[Project](http://hiroharu-kato.com/projects_en/cifar10_3d.html)]

**BlockGAN: Learning 3D Object-Aware Scene Representations from Unlabelled Images.**<br>
*Thu Nguyen-Phuoc, Christian Richardt, Long Mai, Yong-Liang Yang, Niloy Mitra.*<br>
arxiv, 20 Feb 2020. [[PDF](https://arxiv.org/abs/2002.08988)] [[Project](https://www.monkeyoverflow.com/#/blockgan/)]

**DualSDF: Semantic Shape Manipulation using a Two-Level Representation.**<br>
*Zekun Hao, Hadar Averbuch-Elor, Noah Snavely, Serge Belongie.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.02869)]

**Learning a Neural 3D Texture Space from 2D Exemplars.**<br>
*Philipp Henzler, Niloy J. Mitra, Tobias Ritschel.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/1912.04158)] [[Project](https://geometry.cs.ucl.ac.uk/projects/2020/neuraltexture/)]

**Neural Contours: Learning to Draw Lines from 3D Shapes.**<br>
*[Difan Liu](https://people.cs.umass.edu/~dliu/), Mohamed Nabail, [Aaron Hertzmann](https://www.dgp.toronto.edu/~hertzman/), [Evangelos Kalogerakis](https://people.cs.umass.edu/~kalo/).*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.10333)] [[Github](https://github.com/DifanLiu/NeuralContours)]

**Pix2Shape: Towards Unsupervised Learning of 3D Scenes from Images using a View-based Representation.**<br>
*Sai Rajeswar, Fahim Mannan, Florian Golemo, Jérôme Parent-Lévesque, David Vazquez, Derek Nowrouzezahrai, Aaron Courville.*<br>
IJCV 2020. [[PDF](https://arxiv.org/abs/2003.14166)]

**VCN: Volumetric Correspondence Networks for Optical Flow.**<br>
*Gengshan Yang, Deva Ramanan.*<br>
NeurIPS 2019. [[PDF](http://www.contrib.andrew.cmu.edu/~gengshay/wordpress/wp-content/uploads/2019/11/vcn.pdf)] [[GitHub](https://github.com/gengshan-y/VCN)] [[Project](http://www.contrib.andrew.cmu.edu/~gengshay/neurips19flow)]

**Scene Representation Networks: Continuous 3D-Structure-Aware Neural Scene Representations.**<br>
*[Vincent Sitzmann](https://vsitzmann.github.io/), Michael Zollhöfer, Gordon Wetzstein.*<br>
NeurIPS 2019 (Oral, Honorable Mention "Outstanding New Directions").
[[PDF](http://arxiv.org/abs/1906.01618)] [[Project](https://github.com/vsitzmann/scene-representation-networks)] [[Github](https://github.com/vsitzmann/scene-representation-networks)] [[Dataset](https://drive.google.com/drive/folders/1OkYgeRcIcLOFu1ft5mRODWNQaPJ0ps90?usp=sharing)]

**LLFF: Local Light Field Fusion: Practical View Synthesis with Prescriptive Sampling Guidelines.**<br>
*[Ben Mildenhall](http://people.eecs.berkeley.edu/~bmild/), Pratul Srinivasan, Rodrigo Ortiz-Cayon, Nima Khademi Kalantari, Ravi Ramamoorthi, Ren Ng, Abhishek Kar.*<br>
SIGGRAPH 2019. [[PDF](https://arxiv.org/abs/1905.00889)] [[Project](https://people.eecs.berkeley.edu/~bmild/llff/)] [[Github](https://github.com/Fyusion/LLFF)]

**Neural Volumes: Learning Dynamic Renderable Volumes from Images.**<br>
*Stephen Lombardi, Tomas Simon, Jason Saragih, Gabriel Schwartz, Andreas Lehrmann, Yaser Sheikh.*<br>
SIGGRAPH 2019. [[PDF](https://arxiv.org/abs/1906.07751)] [[Github](https://github.com/facebookresearch/neuralvolumes)]

**Transformable Bottleneck Networks.**<br>
*Kyle Olszewski, Sergey Tulyakov, Oliver Woodford, Hao Li, Linjie Luo.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Olszewski_Transformable_Bottleneck_Networks_ICCV_2019_paper.pdf)]

**Equivariant Multi-View Networks.**<br>
*Carlos Esteves, Yinshuang Xu, Christine Allen-Blanchette, Kostas Daniilidis.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1904.00993)]

**DeepVoxels: Learning Persistent 3D Feature Embeddings.**<br>
*Vincent Sitzmann, Justus Thies, Felix Heide, Matthias Nießner, Gordon Wetzstein, Michael Zollhöfer.*<br>
CVPR 2019 (Oral). [[Project](http://vsitzmann.github.io/deepvoxels/)] [[PDF](https://arxiv.org/abs/1812.01024)] [[Code](https://github.com/vsitzmann/deepvoxels)]

**DeepSDF: Learning Continuous Signed Distance Functions for Shape Representation.**<br>
*eong Joon Park, Peter Florence, Julian Straub, Richard Newcombe, Steven Lovegrove.*<br>
CVPR 2019. [[PDF](http://openaccess.thecvf.com/content_CVPR_2019/html/Park_DeepSDF_Learning_Continuous_Signed_Distance_Functions_for_Shape_Representation_CVPR_2019_paper.html)] [[Github](https://github.com/facebookresearch/DeepSDF)]

**Learning View Priors for Single-view 3D Reconstruction.**<br>
*Hiroharu Kato, Tatsuya Harada.*<br>
CVPR 2019. [[PDF](https://arxiv.org/abs/1811.10719)] [[Project](http://hiroharu-kato.com/projects_en/view_prior_learning.html)] [[Github](https://github.com/hiroharu-kato/view_prior_learning)]

**HoloGAN: Unsupervised Learning of 3D Representations from Natural Images.**<br>
*Nguyen-Phuoc, Chuan Li, Lucas Theis, Christian Richardt Yong-liang Yang.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1904.01326)] [[GitHub](https://github.com/christopher-beckham/hologan-pytorch)]

**C3DPO: Canonical 3D Pose Networks for Non-Rigid Structure From Motion.**<br>
*David Novotny, Nikhila Ravi, Benjamin Graham, Natalia Neverova, Andrea Vedaldi.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1909.02533)] [[Github](https://github.com/facebookresearch/c3dpo_nrsfm)] [[Project](https://research.fb.com/publications/c3dpo-canonical-3d-pose-networks-for-non-rigid-structure-from-motion/)]

**CSM: Canonical Surface Mapping via Geometric Cycle Consistency.**<br>
*Nilesh Kulkarni, Abhinav Gupta, Shubham Tulsiani.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1907.10043)] [[Github](https://nileshkulkarni.github.io/csm/)] [[Project](https://nileshkulkarni.github.io/csm/)]

## Representation of Motion

[[6D Pose](https://zhuanlan.zhihu.com/p/94020758?utm_source=wechat_session&utm_medium=social&utm_oi=28410831175680)]

**On the Continuity of Rotation Representations in Neural Networks.**<br>
*Yi Zhou, Connelly Barnes, Jingwan Lu, Jimei Yang, Hao Li.*<br>
CVPR 2019. [[PDF](https://arxiv.org/abs/1812.07035)]

Sparse Representations for Object and Ego-motion Estimation in Dynamic Scenes.*<br>
Hirak J Kashyap, Charless Fowlkes, Jeffrey L Krichmar.*<br>
[[PDF](https://arxiv.org/abs/1903.03731v1)]

CeMNet: Self-supervised Learning For Accurate Continuous Ego-Motion Estimation.*<br>
Minhaeng Lee, Charless C. Fowlkes.*<br>
CVPRW, 2019. [[PDF](https://arxiv.org/abs/1806.10309v1)]

## Surface Cuts and Parameterization 

**OptCuts: Joint Optimization of Surface Cuts and Parameterization.**<br>
*Minchen Li, Danny M. Kaufman, Vladimir G. Kim, Justin Solomon, Alla Sheffer.*<br>
ACM Transactions on Graphics (SIGGRAPH Asia), 2018. [[PDF](http://www.cs.ubc.ca/labs/imager/tr/2018/OptCuts/doc/OptCuts.pdf)] [[Code and Data]()] [[](http://www.cs.ubc.ca/labs/imager/tr/2018/OptCuts/)] 

## Dense Shape Correspondence & Matching

**S2DNet: Learning Accurate Correspondences for Sparse-to-Dense Feature Matching.**<br>
*Hugo Germain, Guillaume Bourmaud, Vincent Lepetit.*<br>
arxiv 2020. [[PDF](https://arxiv.org/pdf/2004.01255.pdf)]

**ANCNet: Correspondence Networks with Adaptive Neighbourhood Consensus.**<br>
*Shuda Li, Kai Han, Theo W. Costain, Henry Howard-Jenkins, Victor Prisacariu.*<br>
CVPR 2020. [[PDF](https://ancnet.avlcode.org/asset/cvpr2020_anc_net.pdf)] [[Project](https://ancnet.avlcode.org/)] [[Github](https://github.com/ActiveVisionLab/ANCNet)] 

**Self-supervised Learning of Dense Shape Correspondence.**<br>
*Oshri Halimi, [Or Litany](https://orlitany.github.io/), Emanuele Rodola, Alex M. Bronstein, Ron Kimmel.*<br>
CVPR 2019 Oral. [[PDF](http://openaccess.thecvf.com/content_CVPR_2019/html/Halimi_Unsupervised_Learning_of_Dense_Shape_Correspondence_CVPR_2019_paper.html)] [[PDF](https://github.com/OshriHalimi/unsupervised_learning_of_dense_shape_correspondence)] 

**Unsupervised Deep Learning for Structured Shape Matching.**<br>
*Jean-Michel Roufosse, Abhishek Sharma, Maks Ovsjanikov.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1812.03794)]

## 3D Reconstruction with Synthesied Images

**Transformable Bottleneck Networks.**<br>
*Kyle Olszewski, Sergey Tulyakov, Oliver Woodford, Hao Li, Linjie Luo.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Olszewski_Transformable_Bottleneck_Networks_ICCV_2019_paper.pdf)]

**SiCloPe: Silhouette-Based Clothed People.**<br>
*Ryota Natsume, [Shunsuke Saito](http://www-scf.usc.edu/~saitos/), Zeng Huang, Weikai Chen, Chongyang Ma, Hao Li, Shigeo Morishima.*<br>
CVPR 2019. [[PDF](http://openaccess.thecvf.com/content_CVPR_2019/papers/Natsume_SiCloPe_Silhouette-Based_Clothed_People_CVPR_2019_paper.pdf)]