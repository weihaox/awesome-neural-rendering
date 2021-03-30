# Learning 3D Representations From Natural Images

This repository is a collection of papers on learning 3D representations from natural images.

## Table of Contents
- [3D Representations From Natural Images](#3d-representations-from-natural-images)
- [3D Shape Representation and Feature Embedding](#3d-shape-representation-and-feature-embedding)
- [Homography Estimation](#homography-estimation)
- [Representation of Texture](#representation-of-texture)
- [Representation of Motion](#representation-of-motion)
- [Surface Cuts and Parameterization](#surface-cuts-and-parameterization)
- [Multi-View or Cross-View Region Matching](#multi-view-or-cross-view-region-matching)
- [Dense Shape Correspondence and Matching](#dense-shape-correspondence-and-matching)
- [3D Reconstruction with Synthesied Images](#3d-reconstruction-with-synthesied-images)

## 3D Representations From Natural Images

**Learning Joint 2D-3D Representations for Depth Completion.**<br>
*Yun Chen, Bin Yang, Ming Liang, Raquel Urtasun.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/2012.12402)]

**Inverse Graphics: Unsupervised Learning of 3D Shapes from Single Images.**<br>
*Talip Ucar.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/1911.07937)]

**Face Video Deblurring Using 3D Facial Priors.**<br>
*Wenqi Ren, Jiaolong Yang, Senyou Deng, David Wipf, Xiaochun Cao, Xin Tong.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Ren_Face_Video_Deblurring_Using_3D_Facial_Priors_ICCV_2019_paper.pdf)]

**TRB: A Novel Triplet Representation for Understanding 2D Human Body.**<br>
*Haodong Duan, Kwan-Yee Lin, Sheng Jin, Wentao Liu, Chen Qian, Wanli Ouyang.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Duan_TRB_A_Novel_Triplet_Representation_for_Understanding_2D_Human_Body_ICCV_2019_paper.pdf)]

**Learning Object-Specific Distance From a Monocular Image.**<br>
*Jing Zhu, Yi Fang.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Zhu_Learning_Object-Specific_Distance_From_a_Monocular_Image_ICCV_2019_paper.pdf)]

**HoloGAN: Unsupervised learning of 3D representations from natural images.**<br>
*Thu Nguyen-Phuoc, Chuan Li, Lucas Theis, Christian Richardt Yong-liang Yang.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1904.01326)] [[GitHub](https://github.com/christopher-beckham/hologan-pytorch)]

**GIFT: Learning Transformation-Invariant Dense Visual Descriptors via Group CNNs.**<br>
*Yuan Liu, Zehong Shen, Zhixuan Lin, Sida Peng, Hujun Bao, Xiaowei Zhou.*<br>
NeurIPS 2019. [[PDF](https://arxiv.org/abs/1911.05932)] [[Github](https://github.com/zju3dv/GIFT)] [[Project](https://zju3dv.github.io/GIFT/)]

**Multi-view Supervision for Single-view Reconstruction via Differentiable Ray Consistency.**<br>
*Shubham Tulsiani, Tinghui Zhou, Alexei A. Efros, Jitendra Malik.*<br>
CVPR 2017 (Oral).[[PDF](https://arxiv.org/abs/1704.06254)]

**Learning View Priors for Single-view 3D Reconstruction.**<br>
*Hiroharu Kato, Tatsuya Harada.*<br>
CVPR 2019. [[PDF](https://arxiv.org/abs/1811.10719)] [[Project](http://hiroharu-kato.com/projects_en/view_prior_learning.html)]

**Self-supervised Learning of 3D Objects from Natural Images.**<br>
*Hiroharu Kato, Tatsuya Harada.*<br>
arxiv 20 Nov 2019. [[PDF](https://arxiv.org/abs/1911.08850)] [[Project](http://hiroharu-kato.com/projects_en/cifar10_3d.html)]

## 3D Shape Representation and Feature Embedding

**PRIN/SPRIN: On Extracting Point-wise Rotation Invariant Features.**<br>
*Yang You, Yujing Lou, Ruoxi Shi, Qi Liu, Yu-Wing Tai, Lizhuang Ma, Weiming Wang, Cewu Lu.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2102.12093)] [[Github](https://github.com/qq456cvb/SPRIN)]

**Deep Implicit Templates for 3D Shape Representation.**<br>
*Zerong Zheng, Tao Yu, Qionghai Dai, Yebin Liu.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.14565)]

**Learning to Compose Hypercolumns for Visual Correspondence.**<br>
*Juhong Min, Jongmin Lee, Jean Ponce, Minsu Cho.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.10587)]

**IMR: Implicit Mesh Reconstruction from Unannotated Image Collections.**<br>
*Shubham Tulsiani, Nilesh Kulkarni, Abhinav Gupta.*<br>
ECCV 2020. [[PDF](https://arxiv.org/pdf/2007.08504.pdf)] [[Project](https://shubhtuls.github.io/imr/)]

**LIMP: Learning Latent Shape Representations with Metric Preservation Priors.**<br>
*Luca Cosmo, Antonio Norelli, Oshri Halimi, Ron Kimmel, Emanuele Rodolà.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2003.12283)]

**Learning 3D Part Assembly from a Single Image.**<br>
*Yichen Li, Kaichun Mo, Lin Shao, Minhyuk Sung, Leonidas Guibas.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2003.09754)]

**Curriculum DeepSDF.**<br>
*Yueqi Duan, Haidong Zhu, He Wang, Li Yi, Ram Nevatia, Leonidas J. Guibas.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2003.08593)] [[Github](https://github.com/haidongz-usc/Curriculum-DeepSDF)]

**NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis.**<br>
*[Ben Mildenhall](http://people.eecs.berkeley.edu/~bmild/), [Pratul P. Srinivasan](https://people.eecs.berkeley.edu/~pratul/), [Matthew Tancik](http://www.matthewtancik.com/), [Jonathan T. Barron](https://jonbarron.info/), [Ravi Ramamoorthi](http://cseweb.ucsd.edu/~ravir/), [Ren Ng](https://www2.eecs.berkeley.edu/Faculty/Homepages/yirenng.html).*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2003.08934)] [[Project](http://tancik.com/nerf)] [[Gtihub-Tensorflow](https://github.com/bmild/nerf)] [[krrish94-PyTorch](https://github.com/krrish94/nerf-pytorch)] [[yenchenlin-PyTorch](https://github.com/yenchenlin/nerf-pytorch)]

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
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.02869)] [[Github](https://github.com/zekunhao1995/DualSDF)]

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

## Homography Estimation

**Content-Aware Unsupervised Deep Homography Estimation.**<br>
*Jirong Zhang, Chuan Wang, Shuaicheng Liu, Lanpeng Jia, Nianjin Ye, Jue Wang, Ji Zhou, Jian Sun.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/1909.05983)] [[Github](https://github.com/JirongZhang/DeepHomography)]

**Unsupervised Deep Homography: A Fast and Robust Homography Estimation Model.**<br>
*Ty Nguyen, Steven W. Chen, Shreyas S. Shivakumar, Camillo J. Taylor, Vijay Kumar.*<br>
IEEE Robotics and Automation Letters 2018. [[PDF](arxiv.org/abs/1709.03966)]

## Representation of Texture

**Neural Texture: Learning a Neural 3D Texture Space from 2D Exemplars.**<br>
*[Henzler](https://henzler.github.io/), [J. Mitra](http://www0.cs.ucl.ac.uk/staff/n.mitra/), [Ritschel](http://www.homepages.ucl.ac.uk/~ucactri/).*<br>
CVPR 2020. [[PDF](https://geometry.cs.ucl.ac.uk/projects/2020/neuraltexture/paper_docs/neuraltexture.pdf)] [[Github](https://github.com/henzler/neuraltexture)]
[[Project](https://geometry.cs.ucl.ac.uk/projects/2020/neuraltexture/)]

## Representation of Motion

[[6D Pose](https://zhuanlan.zhihu.com/p/94020758?utm_source=wechat_session&utm_medium=social&utm_oi=28410831175680)]

**On the Continuity of Rotation Representations in Neural Networks.**<br>
*Yi Zhou, Connelly Barnes, Jingwan Lu, Jimei Yang, Hao Li.*<br>
CVPR 2019. [[PDF](https://arxiv.org/abs/1812.07035)]

**Sparse Representations for Object and Ego-motion Estimation in Dynamic Scenes.**<br>
*Hirak J Kashyap, Charless Fowlkes, Jeffrey L Krichmar.*<br>
TNNLS 2020. [[PDF](https://arxiv.org/abs/1903.03731v1)]

**CeMNet: Self-supervised Learning For Accurate Continuous Ego-Motion Estimation.**<br>
*Minhaeng Lee, Charless C. Fowlkes.*<br>
CVPRW, 2019. [[PDF](https://arxiv.org/abs/1806.10309v1)]

## Surface Cuts and Parameterization 

**OptCuts: Joint Optimization of Surface Cuts and Parameterization.**<br>
*Minchen Li, Danny M. Kaufman, Vladimir G. Kim, Justin Solomon, Alla Sheffer.*<br>
ACM Transactions on Graphics (SIGGRAPH Asia), 2018. [[PDF](http://www.cs.ubc.ca/labs/imager/tr/2018/OptCuts/doc/OptCuts.pdf)] [[Code and Data](http://www.cs.ubc.ca/labs/imager/tr/2018/OptCuts/)] 

## Multi-View or Cross-View Region Matching

**SGP: Self-supervised Geometric Perception.**<br>
*Heng Yang, Wei Dong, Luca Carlone, Vladlen Koltun.*<br>
CVPR 2021. [[PDF](https://github.com/theNded/SGP)] [[Github](https://github.com/theNded/SGP)]

**Descriptor-Free Multi-View Region Matching for Instance-Wise 3D Reconstruction.**<br>
*Takuma Doi, Fumio Okura, Toshiki Nagahara, Yasuyuki Matsushita, Yasushi Yagi.*<br>
ACCV 2020. [[PDF](https://arxiv.org/abs/2011.13649)]

## Dense Shape Correspondence and Matching

**HumanGPS: Geodesic PreServing Feature for Dense Human Correspondences.**<br>
*Feitong Tan, Danhang Tang, Mingsong Dou, Kaiwen Guo, Rohit Pandey, Cem Keskin, Ruofei Du, Deqing Sun, Sofien Bouaziz, Sean Fanello, Ping Tan, Yinda Zhang.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2103.15573)] 

**PDCNet: Learning Accurate Dense Correspondences and When to Trust Them.**<br>
*Prune Truong, Martin Danelljan, Luc Van Gool, Radu Timofte.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2101.01710)] [[Github](https://github.com/PruneTruong/PDCNet)]

**Space-Time Correspondence as a Contrastive Random Walk.**<br>
*Allan Jabri, Andrew Owens, Alexei A. Efros.*<br>
NeurIPS 2020. [[PDF](https://arxiv.org/abs/2006.14613)] [[Github](https://github.com/ajabri/videowalk)] [[Project](https://ajabri.github.io/videowalk/)]

**Patch2Pix: Epipolar-Guided Pixel-Level Correspondences.**<br>
*Qunjie Zhou, Torsten Sattler, Laura Leal-Taixe.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.01909)]

**Dense Correspondences between Human Bodies via Learning Transformation Synchronization on Graphs.**<br>
*Xiangru Huang, Haitao Yang, Etienne Vouga, Qixing Huang.*<br>
NeurIPS 2020. [[PDF](https://www.cs.utexas.edu/~xrhuang/publications/Neurips2020_HumanCorres.pdf)] [[Github](https://github.com/xiangruhuang/HumanCorresViaLearn2Sync)]

**Deep Shells: Unsupervised Shape Correspondence with Optimal Transport.**<br>
*Marvin Eisenberger, Aysim Toker, Laura Leal-Taixé, Daniel Cremers.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2010.15261)]

**Correspondence Matrices are Underrated.**<br>
*Tejas Zodage, Rahul Chakwate, Vinit Sarode, Rangaprasad Arun Srivatsan, Howie Choset.*<br>
3DV 2020. [[PDF](https://arxiv.org/abs/2010.16085)] [[Github](https://github.com/tzodge/PCR-CMU)]

**LoopReg: Self-supervised Learning of Implicit Surface Correspondences, Pose and Shape for 3D Human Mesh Registration.**<br>
*Bharat Lal Bhatnagar, Cristian Sminchisescu, Christian Theobalt, Gerard Pons-Moll.*<br>
NeurIPS 2020. [[PDF](https://arxiv.org/abs/2010.12447)]

**Learning Implicit Functions for Topology-Varying Dense 3D Shape Correspondence.**<br>
*Feng Liu, Xiaoming Liu.*<br>
NeurIPS 2020. [[PDF](https://arxiv.org/abs/2010.12320)]

**Deep Geometric Functional Maps: Robust Feature Learning for Shape Correspondence.**<br>
*Nicolas Donati, Abhishek Sharma, Maks Ovsjanikov.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2003.14286)] [[Github](https://github.com/LIX-shape-analysis/GeomFmaps)]

**D2D: Learning to Find Good Correspondences for Image Matching and Manipulation.**<br>
*Olivia Wiles, Sebastien Ehrhardt, Andrew Zisserman.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2007.08480)]

**Dual-Resolution Correspondence Networks.**<br>
*Xinghui Li, Kai Han, Shuda Li, Victor Adrian Prisacariu.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2006.08844)]

**3D Human Mesh Regression with Dense Correspondence.**<br>
*Wang Zeng, Wanli Ouyang, Ping Luo, Wentao Liu, Xiaogang Wang.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2006.05734)]

**Correspondence Networks with Adaptive Neighbourhood Consensus.**<br>
*Shuda Li, [Kai Han](http://www.hankai.org/), Theo W. Costain, Henry Howard-Jenkins, Victor Prisacariu.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.12059)] [[Project](https://ancnet.avlcode.org/)]

**Facial Action Unit Intensity Estimation via Semantic Correspondence Learning with Dynamic Graph Convolution.**<br>
*Yingruo Fan, Jacqueline C.K. Lam, Victor O.K. Li.*<br>
AAAI 2020. [[PDF](https://arxiv.org/abs/2004.09681)]

**Semantic Correspondence via 2D-3D-2D Cycle.**<br>
*Yang You, Chengkun Li, Yujing Lou, Zhoujun Cheng, Lizhuang Ma, Cewu Lu, Weiming Wang.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2004.09061)] [[Github](https://github.com/qq456cvb/SemanticTransfer)]

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