# Inferring Physical World From Images

A collection of papers on inferring the physical world (shape, depth, motion, paint, light, colors, etc) from single RGB, multi-view or temporal images. 

## Table of Contents
- [Hidden Surface or Object Reasoning](#hidden-surface-or-object-reasoning)
- [Differentiable Physics-Based Simulation and Simulation Platform](#differentiable-physics-based-simulation-and-simulation-platform)
- [Scene Understanding](#scene-understanding)
- [Decomposition and Disentanglement](#decomposition-and-disentanglement)
- [Human Reconstruction: Tissue, Pose, Shape, Dynamic](#human-reconstruction--tissue--pose--shape--dynamic)
  * [Soft-tissue Dynamics](#soft-tissue-dynamics)
  * [Generating 3D People in Scenes](#generating-3d-people-in-scenes)
  * [Shape Interpolation](#shape-interpolation)
  * [3D Pose Transfer](#3d-pose-transfer)
  * [Human Activity and Action Understanding](#human-activity-and-action-understanding)
  * [Human Motion and Dynamics](#human-motion-and-dynamics)
  * [Human Tissue](#human-tissue)
    + [Hair (Subtle) Segmentation and Reconstruction](#hair--subtle--segmentation-and-reconstruction)
    + [Face Reconstruction and Animation](#face-reconstruction-and-animation)
    + [Hand Reconstruction](#hand-reconstruction)
  * [Human Poses and Shapes](#human-poses-and-shapes)
- [Fluid and Smoke Simulation](#fluid-and-smoke-simulation)
- [Object Modeling](#object-modeling)
  * [Reconstruction of Transparent Shapes or Thin Structure](#reconstruction-of-transparent-shapes-or-thin-structure)
  * [Surface Models](#surface-models)
  * [General Object Reconstruction](#general-object-reconstruction)
  * [Object Skeletonization](#object-skeletonization)
  * [Shape and Viewpoint](#shape-and-viewpoint)
- [Pose Estimation](#pose-estimation)
- [Depth Estimation](#depth-estimation)
  * [Dynamic Object](#dynamic-object)
  * [Accurate Edge](#accurate-edge)
  * [Depth From Video (Depth, Normal and Camera Motion Estimation)](#depth-from-video--depth--normal-and-camera-motion-estimation-)
  * [Depth with ToF](#depth-with-tof)
  * [Temporal- and Scale-Consistent Depth Estimation](#temporal--and-scale-consistent-depth-estimation)
  * [Depth and Related Tasks](#depth-and-related-tasks)
- [Learning Temporal Information from Videos](#learning-temporal-information-from-videos)
  * [FastSlow, Multiple Stream and Temporal Pyramid](#fastslow--multiple-stream-and-temporal-pyramid)
  * [3D convolutions (C3D)](#3d-convolutions--c3d-)
  * [Flow](#flow)
  * [2DCNN + LSTM (Temporal Block)](#2dcnn---lstm--temporal-block-)
- [Misc (Speediness, Trajectories)](#misc--speediness--trajectories-)
- [Gaze Estimation, Tracking, Redirection, Correction, and Blink Detection](#gaze-estimation--tracking--redirection--correction-and-blink-detection)
  * [Gaze Dataset](#gaze-dataset)
  * [Gaze Redirection and Correction](#gaze-redirection-and-correction)
  * [Gaze Estimation](#gaze-estimation)
  * [Eye Tracking](#eye-tracking)
- [Team and People](#team-and-people)
- [Good Start of 3D Resources (Python)](#good-start-of-3d-resources--python-)

## Hidden Surface or Object Reasoning

**Object-Centric Diagnosis of Visual Reasoning.**<br>
*Jianwei Yang, Jiayuan Mao, Jiajun Wu, Devi Parikh, David D. Cox, Joshua B. Tenenbaum, Chuang Gan.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.11587)]

**P3I: Perspective Plane Program Induction from a Single Image.**<br>
*[Yikai Li](https://scholar.google.com/citations?view_op=list_works&hl=en&user=5pC7fw8AAAAJ), Jiayuan Mao, Xiuming Zhang, William T. Freeman, Joshua B. Tenenbaum, [Jiajun Wu](https://jiajunwu.com/).*<br>
CVPR 2020. [[PDF](https://jiajunwu.com/papers/p3i_cvpr.pdf)] [[Project](http://p3i.csail.mit.edu/)]

**Footprints and Free Space from a Single Color Image.**<br>
*Jamie Watson, Michael Firman, Aron Monszpart, Gabriel J. Brostow.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.06376)] [[Github](https://github.com/nianticlabs/footprints)]

**Self-Supervised Scene De-occlusion.**<br>
*[Xiaohang Zhan](https://xiaohangzhan.github.io/), Xingang Pan, Bo Dai, Ziwei Liu, Dahua Lin, and Chen Change Loy.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.02788)] [[Github](https://github.com/XiaohangZhan/deocclusion)] [[Project](https://xiaohangzhan.github.io/projects/deocclusion/)] [[Demo](https://www.youtube.com/watch?v=xIHCyyaB5gU)]

**Where Does It End? -- Reasoning About Hidden Surfaces by Object Intersection Constraints.**<br>
*Michael Strecke, Joerg Stueckler.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.04630)]

## Differentiable Physics-Based Simulation and Simulation Platform

**DiffTaichi: Differentiable Programming for Physical Simulation.**<br>
*[Yuanming Hu](http://taichi.graphics/me/), Luke Anderson, Tzu-Mao Li, Qi Sun, Nathan Carr, Jonathan Ragan-Kelley, Fredo Durand.*<br>
ICLR 2020. [[PDF](https://arxiv.org/abs/1910.00935)] [[Github](https://github.com/yuanming-hu/difftaichi)]

**A Physics-based Noise Formation Model for Extreme Low-light Raw Denoising.**<br>
*Kaixuan Wei, Ying Fu, Jiaolong Yang, Hua Huang.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.12751)] [[Github](https://github.com/Vandermode/NoiseModel)]

**Use the Force, Luke! Learning to Predict Physical Forces by Simulating Effects.**<br>
*Kiana Ehsani, Shubham Tulsiani, Saurabh Gupta, Ali Farhadi, Abhinav Gupta.*<br>
CVPR 2020. [[PDF](https://arxiv.org/pdf/2003.12045)]

**SAPIEN: A SimulAted Part-based Interactive ENvironment.**<br>
*[Fanbo Xiang](https://www.fbxiang.com/), [Yuzhe Qin](https://github.com/yzqin), [Kaichun Mo](https://www.cs.stanford.edu/~kaichun/), [Yikuan Xia](https://www.linkedin.com/in/yikuan-xia-4418a9170/), [Hao Zhu](https://berniezhu.github.io/), [Fangchen Liu](https://fangchenliu.github.io/), [Minghua Liu](http://cseweb.ucsd.edu/~mil070/), [Hanxiao Jiang](https://jianghanxiao.github.io/), Yifu Yuan, [He Wang](http://ai.stanford.edu/~hewang/), [Li Yi](https://cs.stanford.edu/~ericyi/), [Angel X. Chang](https://angelxuanchang.github.io/), [Leonidas J. Guibas](http://geometry.stanford.edu/member/guibas/index.html), [Hao Su](https://cseweb.ucsd.edu/~haosu/).*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.08515)] [[Project](https://sapien.ucsd.edu/)] [[Documentation](https://sapien.ucsd.edu/docs/index.html)] [[Github](https://github.com/haosulab/SAPIEN-Release)]

**Differentiable Programming for Physical Simulation.**<br>
*Yuanming Hu, Luke Anderson, Tzu-Mao Li, Qi Sun, Nathan Carr, Jonathan Ragan-Kelley, and Frédo Durand.*<br>
ICLR 2020.  [[PDF](https://arxiv.org/abs/1910.00935)] [[Github](https://github.com/yuanming-hu/taichi)]

**GarNet: A Two-Stream Network for Fast and Accurate 3D Cloth Draping.**<br>
*[Erhan Gundogdu](https://egundogdu.github.io/), Victor Constantin, Amrollah Seifoddini, Minh Dang, Mathieu Salzmann, Pascal Fua.*<br>
ICCV 2019. 
[[PDF](https://arxiv.org/abs/1811.10983)] [[Supplementary Material](https://www.epfl.ch/labs/cvlab/wp-content/uploads/2019/04/GarNet_supplementary.pdf)] 
[[Project](https://cvlab.epfl.ch/research/garment-simulation/garnet/)] [[Dataset](https://drive.switch.ch/index.php/s/7mAk9SoZ7J4uokt)]

**ThreeDWorld: A Platform for Interactive Multi-Modal Physical Simulation.**<br>
*Chuang Gan, Jeremy Schwartz, Seth Alter, Martin Schrimpf, James Traer, Julian De Freitas, Jonas Kubilius, Abhishek Bhandwaldar, Nick Haber, Megumi Sano, Kuno Kim, Elias Wang, Damian Mrowca, Michael Lingelbach, Aidan Curtis, Kevin Feigelis, Daniel M. Bear, Dan Gutfreund, David Cox, James J. DiCarlo, Josh McDermott, Joshua B. Tenenbaum, Daniel L.K. Yamins.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2007.04954)] [[Project](http://www.threedworld.org/)]

**Can I Pour into It? Robot Imagining Open Containability Affordance of Previously Unseen Objects via Physical Simulations.**<br>
*Hongtao Wu, Gregory S. Chirikjian.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.02321)]

## Scene Understanding

**Dark, Beyond Deep: A Paradigm Shift to Cognitive AI with Humanlike Common Sense.**<br>
*Yixin Zhu, Tao Gao, Lifeng Fan, Siyuan Huang, Mark Edmonds, Hangxin Liu, Feng Gao, [Chi Zhang](http://wellyzhang.github.io/), Siyuan Qi, Ying Nian Wu, Joshua B. Tenenbaum, Song-Chun Zhu.*<br>
Engineering 2020. [[PDF](https://arxiv.org/abs/2004.09044)]

**Informative Scene Decomposition for Crowd Analysis, Comparison and Simulation Guidance.**<br>
*Feixiang He, Yuanhang Xiang, Xi Zhao, He Wang.*<br>
SIGGRAPH 2020. [[PDF](https://arxiv.org/abs/2004.14107)]

**Shallow2Deep: Indoor Scene Modeling by Single Image Understanding.**<br>
*Yinyu Nie, Shihui Guo, Jian Chang, Xiaoguang Han, Jiahui Huang, Shi-Min Hu, Jian Jun Zhang.*<br>
Pattern Recognition 2020. [[PDF](https://arxiv.org/abs/2002.09790)]

**Unsupervised Disentanglement of Pose, Appearance and Background from Images and Videos.**<br>
*Aysegul Dundar, Kevin J. Shih, Animesh Garg, Robert Pottorf, Andrew Tao, Bryan Catanzaro.*<br>
arxiv, 26 Jan 2020. [[PDF](https://arxiv.org/abs/2001.09518)]

**3D Dynamic Scene Graphs: Actionable Spatial Perception with Places, Objects, and Humans.**<br>
*Antoni Rosinol, Arjun Gupta, Marcus Abate, Jingnan Shi, Luca Carlone.*<br>
arxiv, 15 Feb 2020. [[PDF](https://arxiv.org/abs/2002.06289)]

**Learning 3D Semantic Scene Graphs from 3D Indoor Reconstructions.**<br>
*Johanna Wald, Helisa Dhamo, Nassir Navab, Federico Tombari.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.03967)]

**Total3DUnderstanding: Joint Layout, Object Pose and Mesh Reconstruction for Indoor Scenes from a Single Image.**<br>
*Yinyu Nie, Xiaoguang Han, Shihui Guo, Yujian Zheng, Jian Chang, Jian Jun Zhang.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2002.12212)]

## Decomposition and Disentanglement

**Physics-based Shading Reconstruction for Intrinsic Image Decomposition.**<br>
*Anil S. Baslamisli, Yang Liu, Sezer Karaoglu, Theo Gevers.*<br>
CVIU 2020. [[PDF](https://arxiv.org/abs/2009.01540)]

**HoliCity: A City-Scale Data Platform for Learning Holistic 3D Structures.**<br>
*Yichao Zhou, Jingwei Huang, Xili Dai, Linjie Luo, Zhili Chen, Yi Ma.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.03286)] [[Project](https://holicity.io/)]

**Weakly Supervised Disentanglement with Guarantees.**<br>
*Rui Shu, Yining Chen, Abhishek Kumar, Stefano Ermon, Ben Poole.*<br>
ICLR 2020. [[PDF](https://openreview.net/forum?id=HJgSwyBKvr)] [[Github](https://github.com/google-research/google-research/tree/master/weak_disentangle)]

**Unsupervised Speech Decomposition via Triple Information Bottleneck.**<br>
*Kaizhi Qian, Yang Zhang, Shiyu Chang, David Cox, Mark Hasegawa-Johnson.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.11284)] [[Project](https://anonymous0818.github.io/)]

**Music Gesture for Visual Sound Separation.**<br>
*Chuang Gan, Deng Huang, Hang Zhao, Joshua B. Tenenbaum, Antonio Torralba.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.09476)] [[Project](http://music-gesture.csail.mit.edu/)]

## Human Reconstruction: Tissue, Pose, Shape, Dynamic

[[Awesome 3D Human Resources List](https://github.com/lijiaman/awesome-3d-human)]

### Soft-tissue Dynamics

**SoftSMPL: Data-driven Modeling of Nonlinear Soft-tissue Dynamics for Parametric Humans.**<br>
*[Igor Santesteban](http://isantesteban.com/), Elena Garces, Miguel A. Otaduy, and Dan Casas.*<br>
Computer Graphics Forum (Proc. of Eurographics), 2020. [[PDF](http://dancasas.github.io/docs/santesteban_Eurographics2020.pdf)] [[Project](http://dancasas.github.io/projects/SoftSMPL)]

### Generating 3D People in Scenes

**PSI: Generating 3D People in Scenes without People.**<br>
*Yan Zhang, Mohamed Hassan, Heiko Neumann, Michael J. Black, Siyu Tang.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/1912.02923)] [[Project](https://ps.is.tuebingen.mpg.de/publications/smpl-x-conditional-vae-prox-scene-constraints)] [[Github](https://github.com/yz-cnsdqz/PSI-release)]

**Synthesizing Long-Term 3D Human Motion and Interaction in 3D Scenes.**<br>
*[Jiashun Wang](https://github.com/jiashunwang), [Huazhe Xu](http://hxu.rocks/), [Jingwei Xu](https://github.com/xjwxjw), [Sifei Liu](https://www.sifeiliu.net/), [Xiaolong Wang](https://xiaolonw.github.io/).*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.05522)] [[Project](https://jiashunwang.github.io/Long-term-Motion-in-3D-Scenes/)]

### Shape Interpolation

**Hamiltonian Dynamics for Real-World Shape Interpolation.**<br>
*Marvin Eisenberger, Daniel Cremers.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2004.05199)]

### 3D Pose Transfer

**Neural Pose Transfer by Spatially Adaptive Instance Normalization.**<br>
*Jiashun Wang, Chao Wen, Yanwei Fu, Haitao Lin, Tianyun Zou, Xiangyang Xue, Yinda Zhang.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.07254)] [[Github](https://github.com/jiashunwang/Neural-Pose-Transfer)]

### Human Activity and Action Understanding

HAKE: Human Activity Knowledge Engine. [MVIG](http://hake-mvig.cn/home/) - Shanghai Jiao Tong University.

**Detailed 2D-3D Joint Representation for Human-Object Interaction.**<br>
*Yong-Lu Li, Xinpeng Liu, Han Lu, Shiyi Wang, Junqi Liu, Jiefeng Li, Cewu Lu.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.08154)] [[Github](https://github.com/DirtyHarryLYL/DJ-RN)]

**PaStaNet: Toward Human Activity Knowledge Engine.**<br>
*Yong-Lu Li, Liang Xu, Xinpeng Liu, Xijie Huang, Yue Xu, Shiyi Wang, Hao-Shu Fang, Ze Ma, Mingyang Chen, Cewu Lu.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.00945)] [[Github](http://hake-mvig.cn/)]

### Human Motion and Dynamics 

**Learning Complex 3D Human Self-Contact.**<br>
*Mihai Fieraru, Mihai Zanfir, Elisabeta Oneata, Alin-Ionut Popa, Vlad Olaru, Cristian Sminchisescu.*<br>
AAAI 2021. [[PDF](https://arxiv.org/abs/2012.10366)]

**iMoCap: Motion Capture from Internet Videos.**<br>
*Junting Dong, Qing Shuai, Yuanqing Zhang, Xian Liu, Xiaowei Zhou, Hujun Bao.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2008.07931)] [[Project](https://zju3dv.github.io/iMoCap/)]
 
**Contact and Human Dynamics from Monocular Video.**<br>
*Davis Rempe, Leonidas J. Guibas, Aaron Hertzmann, Bryan Russell, Ruben Villegas, Jimei Yang.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.11678)]

**Weakly-supervised Learning of Human Dynamics.**<br>
*Petrissa Zell, Bodo Rosenhahn, Bastian Wandt.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.08969)]

**MotioNet: 3D Human Motion Reconstruction from Monocular Video with Skeleton Consistency.**<br>
*[Mingyi Shi](https://rubbly.cn/), [Kfir Aberman](http://kfiraberman.github.io/), [Andreas Aristidou](http://andreasaristidou.com/), [Taku Komura](http://homepages.inf.ed.ac.uk/tkomura/), [Dani Lischinski](https://www.cse.huji.ac.il/~danix/), [Daniel Cohen-Or](https://www.cs.tau.ac.il/~dcor/), [Baoquan Chen](https://cfcs.pku.edu.cn/baoquan).*<br>
TOG 2020. [[PDF](https://arxiv.org/abs/2006.12075)] [[Project](https://rubbly.cn/publications/motioNet)] [[Github](https://github.com/Shimingyi/MotioNet)]

**Deep 3D Capture: Geometry and Reflectance from Sparse Multi-View Images.**<br>
*Sai Bi, Zexiang Xu, Kalyan Sunkavalli, David Kriegman, Ravi Ramamoorthi.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.12642)]

**Do As I Do: Transferring Human Motion and Appearance between Monocular Videos with Spatial and Temporal Constraints.**<br>
*Thiago L. Gomes, Renato Martins, João Ferreira, Erickson R. Nascimento.*<br>
WACV 2020. [[PDF](https://arxiv.org/abs/2001.02606)]

**NASA: Neural Articulated Shape Approximation.**<br>
*Timothy Jeruzalski, Boyang Deng, Mohammad Norouzi, JP Lewis, Geoffrey Hinton, Andrea Tagliasacchi.*<br>
arxiv, 6 Dec 2019. [[PDF](https://arxiv.org/abs/1912.03207)]

**VIBE: Video Inference for Human Body Pose and Shape Estimation.**<br>
*Muhammed Kocabas, Nikos Athanasiou, Michael J. Black.*<br>
arxiv, 11 Dec 2019. [[PDF](https://arxiv.org/abs/1912.05656)]

**Learning 3D Human Dynamics from Video.**<br>
*Angjoo Kanazawa, Jason Y. Zhang, Panna Felsen, Jitendra Malik.*<br>
CVPR 2019. [[PDF](https://arxiv.org/abs/1812.01601)] [[Project](https://akanazawa.github.io/human_dynamics/)]

**Predicting 3D Human Dynamics from Video.**<br>
*Jason Y. Zhang, Panna Felsen, Angjoo Kanazawa, Jitendra Malik.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1908.04781)] [[Project](https://jasonyzhang.com/phd/)]

**DeepHuman: 3D Human Reconstruction from a Single Image.**<br>
*[Zerong Zheng](https://zhengzerong.github.io/), [Tao Yu](https://ytrock.com/), Yixuan Wei, Qionghai Dai, [Yebin Liu](http://www.liuyebin.com/).*<br>
ICCV 2019. [[PDF](http://www.liuyebin.com/deephuman/assets/DeepHuman.pdf)] [[Project](http://www.liuyebin.com/deephuman/deephuman.html)] [[Code](https://github.com/ZhengZerong/DeepHuman)] [[THUmanDataset](https://github.com/ZhengZerong/DeepHuman/tree/master/THUmanDataset)] [[im2smpl](https://github.com/ZhengZerong/im2smpl)]

**LiveCap: Real-time Human Performance Capture from Monocular Video.**<br>
*Marc Habermann, Weipeng Xu, Michael and Zollhoefer, Gerard Pons-Moll, Christian Theobalt.*<br>
SIGGRAPH 2019. [[PDF](https://gvv.mpi-inf.mpg.de/projects/LiveCap/)] [[Project](https://gvv.mpi-inf.mpg.de/projects/LiveCap/)]

**Superpixel Soup: Monocular Dense 3D Reconstruction of a Complex Dynamic Scene.**<br>
*Suryansh Kumar, Yuchao Dai, Hongdong Li.*<br>
TPAMI 2019 (ICCV 2017). [[PDF](https://arxiv.org/abs/1911.09092)] 

### Human Tissue

#### Hair (Subtle) Segmentation and Reconstruction

**Semantic Soft Segmentation.**<br>
*Yagiz Aksoy, Tae-Hyun Oh, Sylvain Paris, Marc Pollefeys and Wojciech Matusik.*<br>
ACM Transactions on Graphics (Proc. SIGGRAPH), 2018. [[PDF](http://yaksoy.github.io/papers/TOG18-sss-supp.pdf)] [[Project](http://yaksoy.github.io/sss/)] [[Github](https://github.com/yaksoy/SemanticSoftSegmentation)] 

**Soft Segmentation of Images.**<br>
*Yagiz Aksoy.*<br>
PhD Thesis, ETH Zurich, 2019. [[PDF](http://yaksoy.github.io/papers/ETH19-PhD-Aksoy.pdf)] [[Project](yaksoy.github.io/ssi/)]

**Meticulous Object Segmentation.**<br>
*Chenglin Yang, Yilin Wang, Jianming Zhang, He Zhang, Zhe Lin, Alan Yuille.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.07181)]

**MODNet: Is a Green Screen Really Necessary for Real-Time Human Matting?**<br>
*Zhanghan Ke, Kaican Li, Yurou Zhou, Qiuhua Wu, Xiangyu Mao, Qiong Yan, Rynson W.H. Lau.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.11961)] [[GitHub](https://github.com/ZHKKKe/MODNet)]

**Dynamic Hair Modeling from Monocular Videos using Deep Neural Networks.**<br>
*Lingchen Yang, Zefeng Shi, [Youyi Zheng](http://youyizheng.net/research.html), [Kun Zhou](http://kunzhou.net/).*<br>
ACM Transactions on Graphics (SIGGRAPH ASIA 2019). [[PDF](http://www.cad.zju.edu.cn/home/zyy/docs/dynamic_hair.pdf)]

**Hair-GAN: Recovering 3D Hair Structure from a Single Image using Generative Adversarial Networks.**<br>
*Meng Zhang, Youyi Zheng.*<br>
Visual Informatics 2019. [[PDF](http://www.cad.zju.edu.cn/home/zyy/docs/hairgan_final.pdf)]

**Learning-based Sampling for Natural Image Matting.**<br>
*Jingwei Tang, Yagiz Aksoy, Cengiz Oztireli, Markus Gross, and Tunc Ozan Aydin.*<br>
CVPR, 2019. [[PDF](http://yaksoy.github.io/papers/CVPR19-samplenet.pdf)] [[Project](http://yaksoy.github.io/samplenet/)] 

**3D Hair Synthesis Using Volumetric Variational Autoencoders.**<br>
*Shunsuke Saito, Liwen Hu, Chongyang Ma, Hikaru Ibayashi, Linjie Luo, Hao Li.*<br>
ACM Transaction on Graphics (SIGGRAPH Asia 2018). [[PDF](http://www.hao-li.com/publications/papers/siggraphAsia2018PAGAN.pdf)]

**HairNet: Single-View Hair Reconstruction using Convolutional Neural Networks.**<br>
*Yi Zhou, Liwen Hu, Jun Xing, Weikai Chen, Han-Wei Kung, Xin Tong, Hao Li.*<br>
arxiv 2018. [[PDF](https://arxiv.org/abs/1806.07467)] [[GitHub](https://github.com/papagina/HairNet_orient2D)] [[GitHub](https://github.com/papagina/HairNet_DataSetGeneration)]

#### Face Reconstruction and Animation

**MeInGame: Create a Game Character Face from a Single Portrait.**<br>
*Jiangke Lin, Yi Yuan, Zhengxia Zou.*<br>
AAAI 2021. [[PDF](https://arxiv.org/abs/2102.02371)]

**Practical Face Reconstruction via Differentiable Ray Tracing.**<br>
*Abdallah Dib, Gaurav Bharaj, Junghyun Ahn, Cédric Thébault, Philippe-Henri Gosselin, Marco Romeo, Louis Chevallier.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2101.05356)]

**Shape My Face: Registering 3D Face Scans by Surface-to-Surface Translation.**<br>
*Mehdi Bahri, Eimear O' Sullivan, Shunwang Gong, Feng Liu, Xiaoming Liu, Michael M. Bronstein, Stefanos Zafeiriou.*<br>
IJCV Submission. [[PDF](https://arxiv.org/abs/2012.09235)]

**High-Fidelity 3D Digital Human Creation from RGB-D Selfies.**<br>
*Xiangkai Lin, Yajing Chen, Linchao Bao, Haoxian Zhang, Sheng Wang, Xuefei Zhe, Xinwei Jiang, Jue Wang, Dong Yu, and Zhengyou Zhang.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2010.05562)] [[Github](https://github.com/tencent-ailab/hifi3dface)] [[Project](https://tencent-ailab.github.io/hifi3dface_projpage/)]

**MGCNet: Self-Supervised Monocular 3D Face Reconstruction by Occlusion-Aware Multi-view Geometry Consistency.**<br>
*Jiaxiang Shang, Tianwei Shen, Shiwei Li, Lei Zhou, Mingmin Zhen, Tian Fang, Long Quan.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.12494)] [[Github](https://github.com/jiaxiangshang/MGCNet)]

**DFNRMVS: Deep Facial Non-Rigid Multi-View Stereo.**<br>
*Ziqian Bai, Zhaopeng Cui, Jamal Ahmed Rahim, Xiaoming Liu, Ping Tan.*<br>
CVPR 2020. [[PDF](https://openaccess.thecvf.com/content_CVPR_2020/papers/Bai_Deep_Facial_Non-Rigid_Multi-View_Stereo_CVPR_2020_paper.pdf)] [[Github](https://github.com/zqbai-jeremy/DFNRMVS)]

**Accurate 3D Face Reconstruction with Weakly-Supervised Learning: From Single Image to Image Set.**<br>
*Yu Deng, Jiaolong Yang, Sicheng Xu, Dong Chen, Yunde Jia, Xin Tong.*<br>
CVPRW on Analysis and Modeling of Faces and Gestures (AMFG), 2019. (Best Paper Award) [[PDF](https://arxiv.org/abs/1903.08527)] [[Github](https://github.com/microsoft/Deep3DFaceReconstruction)]

**Towards Fast, Accurate and Stable 3D Dense Face Alignment.**<br>
*Jianzhu Guo, Xiangyu Zhu, Yang Yang, Fan Yang, Zhen Lei, Stan Z. Li.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2009.09960)] [[Github](https://github.com/cleardusk/3DDFA_V2)]

**Audio- and Gaze-driven Facial Animation of Codec Avatars.**<br>
*Alexander Richard, Colin Lea, Shugao Ma, Juergen Gall, Fernando de la Torre, Yaser Sheikh.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.05023)] [[Project](https://research.fb.com/videos/audio-and-gaze-driven-facial-animation-of-codec-avatars/)]

**TBGAN: Synthesizing Coupled 3D Face Modalities by Trunk-Branch Generative Adversarial Networks.**<br>
*Baris Gecer, Alexander Lattas, Stylianos Ploumpis, Jiankang Deng, Athanasios Papaioannou, Stylianos Moschoglou, Stefanos Zafeiriou.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/1909.02215)] [[Project](https://github.com/barisgecer/TBGAN)]

**Disentangled and Controllable Face Image Generation via 3D Imitative-Contrastive Learning.**<br>
*Yu Deng, Jiaolong Yang, Dong Chen, Fang Wen, Xin Tong.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.11660)]

**Deep 3D Portrait from a Single Image.**<br>
*Sicheng Xu, Jiaolong Yang, Dong Chen, Fang Wen, Yu Deng, Yunde Jia, Xin Tong.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.11598)] [[Github](https://github.com/sicxu/Deep3dPortrait)]

**Adaptive 3D Face Reconstruction from a Single Image.**<br>
*Kun Li, Jing Yang, Nianhong Jiao, Jinsong Zhang, Yu-Kun Lai.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2007.03979)]

**Real-Time Monocular 4D Face Reconstruction using the LSFM Models.**<br>
*Mohammad Rami Koujan, Nikolai Dochev, Anastasios Roussos.*<br>
ACM SIGGRAPH European Conference on Visual Media Production 2020. [[PDF](https://arxiv.org/abs/2006.10499)]

**FaceScape: a Large-scale High Quality 3D Face Dataset and Detailed Riggable 3D Face Prediction.**<br>
*Haotian Yang, Hao Zhu, Yanru Wang, Mingkai Huang, Qiu Shen, Ruigang Yang, Xun Cao.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.13989)] [[Github](https://github.com/zhuhao-nju/facescape)] [[Github](https://github.com/yanght321/Detailed3DFace)]

**A Morphable Face Albedo Model.**<br>
*William A.P. Smith, Alassane Seck, Hannah Dee, Bernard Tiddeman, Joshua Tenenbaum, Bernhard Egger.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.02711)]

**Rotate-and-Render: Unsupervised Photorealistic Face Rotation from Single-View Images.**<br>
*Hang Zhou, Jihao Liu, Ziwei Liu, Yu Liu, Xiaogang Wang.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.08124)] [[Github](https://github.com/Hangz-nju-cuhk/Rotate-and-Render)]

**Towards High-Fidelity 3D Face Reconstruction from In-the-Wild Images Using Graph Convolutional Networks.**<br>
*Jiangke Lin, Yi Yuan, Tianjia Shao, Kun Zhou.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.05653)]

**Semi-Supervised Monocular 3D Face Reconstruction With End-to-End Shape-Preserved Domain Transfer.**<br>
*Jingtan Piao, Chen Qian, Hongsheng Li.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Piao_Semi-Supervised_Monocular_3D_Face_Reconstruction_With_End-to-End_Shape-Preserved_Domain_Transfer_ICCV_2019_paper.pdf)]

**FML: Face Model Learning From Video.**<br>
*A. Tewari, F. Bernard, P. Garrido, G. Bharaj, M. Elgharib, H-P. Seidel, P. Perez, M. Zollhöfer, C.Theobalt.*  <br>
CVPR 2019. [[PDF](http://gvv.mpi-inf.mpg.de/projects/FML19/paper.pdf)] [[MPI Informatics, Saarland Informatics Campus](http://www.mpi-inf.mpg.de/home/)] [[Project](gvv.mpi-inf.mpg.de/projects/FML19)] 

**FacePSNet: Lightweight Photometric Stereo for Facial Details Recovery.**<br>
*Xueying Wang, Yudong Guo, Bailin Deng, Juyong Zhang.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.12307)] [[Github](https://github.com/Juyong/FacePSNet)]

**High Accuracy Face Geometry Capture using a Smartphone Video.**<br>
*Shubham Agrawal, Anuj Pahuja, Simon Lucey.*<br>
WACV 2020. [[PDF](https://arxiv.org/abs/2003.08583)]

**AvatarMe: Realistically Renderable 3D Facial Reconstruction "in-the-wild".**<br>
*Alexandros Lattas, Stylianos Moschoglou, Baris Gecer, Stylianos Ploumpis, Vasileios Triantafyllou, Abhijeet Ghosh, Stefanos Zafeiriou.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.13845)] [[Github](http://github.com/lattas/AvatarMe)]

#### Hand or Hand-Object Joint Reconstruction

**Unsupervised Domain Adaptation with Temporal-Consistent Self-Training for 3D Hand-Object Joint Reconstruction.**<br>
*Mengshi Qi, Edoardo Remelli, Mathieu Salzmann, Pascal Fua.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.11260)]

**HandVoxNet: Deep Voxel-Based Network for 3D Hand Shape and Pose Estimation from a Single Depth Map.**<br>
*Jameel Malik, Ibrahim Abdelaziz, Ahmed Elhayek, Soshi Shimada, Sk Aziz Ali, Vladislav Golyanik, Christian Theobalt, Didier Stricker.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.01588)]

**Learning Joint Reconstruction of Hands and Manipulated Objects.**<br>
*Yana Hasson, Gül Varol, Dimitris Tzionas, Igor Kalevatykh, Michael J. Black, Ivan Laptev, Cordelia Schmid.*<br>
CVPR 2019. [[PDF](https://arxiv.org/abs/1904.05767)] [[Project](https://hassony2.github.io/obman.html)] [[ObMan dataset](https://github.com/hassony2/obman)] [[Github](https://github.com/hassony2/obman_train)]

**Leveraging Photometric Consistency over Time for Sparsely Supervised Hand-Object Reconstruction.**<br>
*Yana Hasson, Bugra Tekin, Federica Bogo, Ivan Laptev, Marc Pollefeys, Cordelia Schmid.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.13449)] [[Project](https://hassony2.github.io/handobjectconsist.html)]

**DeepHandMesh: A Weakly-supervised Deep Encoder-Decoder Framework for High-fidelity Hand Mesh Modeling.**<br>
*Gyeongsik Moon, Takaaki Shiratori, Kyoung Mu Lee.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2008.08213)] [[Project](https://mks0601.github.io/DeepHandMesh/)]

### Human Poses and Shapes

**Pose2Mesh: Graph Convolutional Network for 3D Human Pose and Mesh Recovery from a 2D Human Pose.**<br>
*Hongsuk Choi, Gyeongsik Moon, Kyoung Mu Lee.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2008.09047)] [[Github](https://github.com/hongsukchoi/Pose2Mesh_RELEASE)]

**ExPose: Monocular Expressive Body Regression through Body-Driven Attention.**<br>
*Vasileios Choutas, Georgios Pavlakos, Timo Bolkart, Dimitrios Tzionas, Michael J. Black.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.09062)] [[Project](https://expose.is.tue.mpg.de/)]

**Human Body Model Fitting by Learned Gradient Descent.**<br>
*Jie Song, Xu Chen, [Otmar Hilliges](https://ait.ethz.ch/people/hilliges/).*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.08474)]

**Perceiving 3D Human-Object Spatial Arrangements from a Single Image in the Wild.**<br>
*Jason Y. Zhang, Sam Pepose, Hanbyul Joo, Deva Ramanan, Jitendra Malik, Angjoo Kanazawa.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.15649)]

**Unsupervised Shape and Pose Disentanglement for 3D Meshes.**<br>
*Keyang Zhou, Bharat Lal Bhatnagar, Gerard Pons-Moll.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.11341)] [[Github](https://virtualhumans.mpi-inf.mpg.de/unsup_shape_pose/)]

**3D Human Shape Reconstruction from a Polarization Image.**<br>
*Shihao Zou, Xinxin Zuo, Yiming Qian, Sen Wang, Chi Xu, Minglun Gong, Li Cheng.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.09268)]

**DecoMR: 3D Human Mesh Regression with Dense Correspondence.**<br>
*Wang Zeng, Wanli Ouyang, Ping Luo, Wentao Liu, Xiaogang Wang.*<br>
CVPR 2020. [[PDF](https://arxiv.org/pdf/2006.05734.pdf)] [[Github](https://github.com/zengwang430521/DecoMR)] [[GraphCMR](https://github.com/nkolot/GraphCMR)] [[DenseBody](https://github.com/Lotayou/densebody_pytorch)]

**Coherent Reconstruction of Multiple Humans from a Single Image.**<br>
*[Wen Jiang](https://jiangwenpl.github.io/), [Nikos Kolotouros](https://www.seas.upenn.edu/~nkolot), [Georgios Pavlakos](https://www.seas.upenn.edu/~pavlakos), [Xiaowei Zhou](http://www.cad.zju.edu.cn/home/xzhou), [Kostas Daniilidis](https://www.cis.upenn.edu/~kostas).*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2006.08586)] [[Project](https://jiangwenpl.github.io/multiperson/)]

**DecoMR: 3D Human Mesh Regression with Dense Correspondence.**<br>
*Wang Zeng, Wanli Ouyang, Ping Luo, Wentao Liu, Xiaogang Wang.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2006.05734)] [[Github](https://github.com/zengwang430521/DecoMR)]

**Bodies at Rest: 3D Human Pose and Shape Estimation from a Pressure Image using Synthetic Data.**<br>
*Henry M. Clever, Zackory Erickson, Ariel Kapusta, Greg Turk, C. Karen Liu, Charles C. Kemp.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.01166)]

**PoseNet3D: Unsupervised 3D Human Shape and Pose Estimation.**<br>
*Shashank Tripathi, Siddhant Ranade, Ambrish Tyagi, Amit Agrawal.*<br>
arxiv, 2020. [[PDF](https://arxiv.org/abs/2003.03473)]

**MoVi: A Large Multipurpose Motion and Video Dataset.**<br>
*Saeed Ghorbani, Kimia Mahdaviani, Anne Thaler, Konrad Kording, Douglas James Cook, Gunnar Blohm, Nikolaus F. Troje.*<br>
arxiv, 4 Mar 2020. [[PDF](https://arxiv.org/abs/2003.01888)]

**Chained Representation Cycling: Learning to Estimate 3D Human Pose and Shape by Cycling Between Representations.**<br>
*Nadine Rueegg, Christoph Lassner, Michael J. Black, Konrad Schindler.*<br>
AAAI 2020. [[PDF](https://arxiv.org/abs/2001.01613)]

**A Skeleton-bridged Deep Learning Approach for Generating Meshes of Complex Topologies from Single RGB Images.**<br>
*Jiapeng Tang, Xiaoguang Han, Junyi Pan, Kui Jia, Xin Tong.*<br>
CVPR 2019. [[PDF](https://arxiv.org/abs/1903.04704)]

**Learning 3D Human Shape and Pose from Dense Body Parts.**<br>
*Hongwen Zhang, Jie Cao, Guo Lu, Wanli Ouyang, Zhenan Sun.*<br>
arxiv, 2019. 
[[PDF](https://hongwenzhang.github.io/dense2mesh/pdf/learning3Dhuman.pdf)]
[[Project](https://hongwenzhang.github.io/dense2mesh)]

**Chained Representation Cycling: Learning to Estimate 3D Human Pose and Shape by Cycling Between Representations.**<br>
*Nadine Rueegg, Christoph Lassner, Michael J. Black, Konrad Schindler.*<br>
AAAI 2020. [[PDF](https://arxiv.org/abs/2001.01613)] [[Project](https://ps.is.tuebingen.mpg.de/publications/ruegg-aaai-2020)]

**Human Mesh Recovery From Monocular Images via a Skeleton-Disentangled Representation.**<br>
*Yu Sun, Yun Ye, Wu Liu, Wenpeng Gao, Yili Fu, Tao Mei.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Sun_Human_Mesh_Recovery_From_Monocular_Images_via_a_Skeleton-Disentangled_Representation_ICCV_2019_paper.pdf)] [[Github](https://github.com/Arthur151/DSD-SATN)]

**HMR: End-to-end Recovery of Human Shape and Pose.**<br>
*Angjoo Kanazawa, Michael J. Black, David W. Jacobs, Jitendra Malik.*<br><br>
CVPR 2018. [[PDF](https://arxiv.org/abs/1712.06584)] [[Github](https://github.com/MandyMo/pytorch_HMR)] [[Project](https://akanazawa.github.io/hmr/)]

**Keep It SMPL: Automatic Estimation of 3D Human Pose and Shape from a Single Image.**<br>
*Federica Bogo*, Angjoo Kanazawa*, Christoph Lassner, Peter Gehler, Javier Romero, Michael Black.*<br>
ECCV 2016. [[Project](http://smplify.is.tue.mpg.de/)] [[PDF](https://www.semanticscholar.org/paper/Keep-It-SMPL%3A-Automatic-Estimation-of-3D-Human-Pose-Bogo-Kanazawa/4233b07033a1ef8af188383f30602a5fd0aa2181)]

**SMPL: A Skinned Multi-Person Linear Model.**<br>
*Matthew Loper, Naureen Mahmood, Javier Romero, Gerard Pons-Moll, Michael J. Black.*<br>
ACM Trans. Graphics (Proc. SIGGRAPH Asia) 2016. [[PDF](http://files.is.tue.mpg.de/black/papers/SMPL2015.pdf)] [[Offical](https://smpl.is.tue.mpg.de/)] [[SMPL layer for PyTorch](https://github.com/gulvarol/smplpytorch)]

## Fluid and Smoke Simulation

**DUDE: Deep Unsigned Distance Embeddings for Hi-Fidelity Representation of Complex 3D Surfaces.**<br>
*Rahul Venkatesh, Sarthak Sharma, Aurobrata Ghosh, Laszlo Jeni, Maneesh Singh.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.02570)]

**RBF Liquids: An Adaptive PIC Solver Using RBF-FD.**<br>
*Rafael Nakanishi Filipe Nascimento Rafael Campos Paulo Pagliosa Afonso Paiva.*<br>
Siggraph Asia 2020 | ACM Transactions on Graphics. [[PDF](https://rnakanishi.github.io/publications/rbf-liquids-adaptive-pic-solver-using-rbf/)] 

**3D Fluid Flow Reconstruction Using Compact Light Field PIV.**<br>
*Zhong Li, Yu Ji, Jingyi Yu, Jinwei Ye.*<br>
ECCV 2020. [[pdf](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123610120.pdf)] [[Supplement](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123610120-supp.zip)]

**Wave Curves: Simulating Lagrangian Water Waves on Dynamically Deforming Surfaces.**<br>
*Tomas Skrivan, Andreas Soderstrom, John Johansson, Christoph Sprenger, Ken Museth, [Chris Wojtan](http://pub.ist.ac.at/group_wojtan/index.html).*<br>
ACM Transactions on Graphics (SIGGRAPH 2020). [[PDF](http://pub.ist.ac.at/group_wojtan/projects/2020_Skrivan_WaveCurves/wave_curves_2020.pdf)]

**Constraint Bubbles and Affine Regions: Reduced Fluid Models for Efficient Immersed Bubbles and Flexible Spatial Coarsening.**<br>
*Ryan Goldade, Mridul Aanjaneya, Christopher Batty.*<br>
TOG 2020. [[PDF](https://cs.uwaterloo.ca/~c2batty/papers/Goldade2020/reduced_fluids.pdf)] [[Project](https://cs.uwaterloo.ca/~rgoldade/reducedfluids/)] [[Github](https://github.com/rgoldade/ReducedFluids)]

**Chemomechanical Simulation of Soap Film Flow on Spherical Bubbles.**<br>
*Weizhen Huang, Julian Iseringhausen, Tom Kneiphof, Ziyin Qu, Chenfanfu Jiang, Matthias B. Hullin.*<br>
TOG 2020. [[PDF](https://light.cs.uni-bonn.de/papers/HuangEtAl-SoapBubbles-SIGGRAPH2020.pdf)] [[Project](https://light.cs.uni-bonn.de/chemomechanical-simulation-of-soap-film-flow-on-spherical-bubbles/)]

**Fast and Scalable Turbulent Flow Simulation with Two-Way Coupling.**<br>
*Wei Li, Yixin Chen, Mathieu Desbrun, Changxi Zhang, Xiaopei Liu.*<br>
SIGGRAPH 2020. [[PDF](http://www.geometry.caltech.edu/pubs/LCDZL20.pdf)]

**Lagrangian Neural Style Transfer for Fluids.**<br>
*Byungsoo Kim, Vinicius C. Azevedo, Markus Gross, Barbara Solenthaler.*<br>
SIGGRAPH 2020. [[PDF](https://arxiv.org/abs/2005.00803)]

**Transport-Based Neural Style Transfer for Smoke Simulations.**<br>
*Byungsoo Kim, Vinicius C. Azevedo, Markus Gross, Barbara Solenthaler.*<br>
SIGGRAPH ASIA 2019. [[PDF](https://arxiv.org/abs/1905.07442)]

**Constraint Bubbles and Affine Regions: Reduced Fluid Models for Efficient Immersed Bubbles and Flexible Spatial Coarsening.**<br>
*Ryan Goldade, Mridul Aanjaneya, Christopher Batty.*<br>
SIGGRAPH 2020. [[PDF](https://cs.uwaterloo.ca/~c2batty/papers/Goldade2020/reduced_fluids.pdf)]

## Object Modeling

CVPR 2020 Workshop on Deep Learning Foundations of Geometric Shape Modeling and Reconstruction. [[Video](http://t.cn/A6LmLlgL)]

### Reconstruction of Deformable or Non-rigid Objects

**Neural Deformation Graphs for Globally-consistent Non-rigid Reconstruction.**<br>
*Aljaž Božič, Pablo Palafox, Michael Zollhöfer, Justus Thies, Angela Dai, Matthias Nießner.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.01451)] [[Video](https://youtu.be/vyq36eFkdWo)]

### Reconstruction of Transparent Shapes or Thin Structure

**GeLaTO: Generative Latent Textured Objects.**<br>
*Ricardo Martin-Brualla, Rohit Pandey, Sofien Bouaziz, Matthew Brown, Dan B Goldman.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2008.04852)] [[Project](https://gelato-paper.github.io/)]

**Vid2Curve: Simultaneously Camera Motion Estimation and Thin Structure Reconstruction from an RGB Video.**<br>
*Peng Wang, Lingjie Liu, Nenglun Chen, Hung-Kuo Chu, Christian Theobalt, Wenping Wang.*<br>
SIGGRAPH 2020. [[PDF](https://arxiv.org/abs/2005.03372)] [[Github](https://github.com/Totoro97/Vid2Curve)]

**ClearGrasp: 3D Shape Estimation of Transparent Objects for Manipulation.**<br>
*Shreeyak S. Sajjan, Matthew Moore, Mike Pan, Ganesh Nagaraja, Johnny Lee, Andy Zeng, Shuran Song.*<br>
[[PDF](https://arxiv.org/abs/1910.02550)] [[Github](https://github.com/Shreeyak/cleargrasp)] [[Project](https://sites.google.com/view/cleargrasp)]

**Through the Looking Glass: Neural 3D Reconstruction of Transparent Shapes.**<br>
*Zhengqin Li, Yu-Ying Yeh, Manmohan Chandraker.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.10904)]

### Surface Models

**Learning Category-level Shape Saliency via Deep Implicit Surface Networks.**<br>
*Chaozheng Wu, Lin Sun, Xun Xu, Kui Jia.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.07290)]

**Topology-Adaptive Mesh Deformation for Surface Evolution, Morphing, and Multi-View Reconstruction.**<br>
*Andrei Zaharescu, Edmond Boyer, Radu Horaud.*<br>
TPAMI 2021. [[PDF](https://arxiv.org/abs/2012.05536)]

**Diffusion is All You Need for Learning on Surfaces.**<br>
*Nicholas Sharp, Souhaib Attaiki, Keenan Crane, Maks Ovsjanikov.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.00888)]

**Continuous Surface Embeddings.**<br>
*Natalia Neverova, David Novotny, Vasil Khalidov, Marc Szafraniec, Patrick Labatut, Andrea Vedaldi.*<br>
NeurIPS 2020. [[PDF](https://arxiv.org/abs/2011.12438)]

**Deep Active Surface Models.**<br>
*Udaranga Wickramasinghe, Graham Knott, Pascal Fua.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.08826)]

**Pix2Surf: Learning Parametric 3D Surface Models of Objects from Images.**<br>
*Jiahui Lei, Srinath Sridhar, Paul Guerrero, Minhyuk Sung, Niloy Mitra, Leonidas J. Guibas.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2008.07760)]

**Surface Normals and Shape From Water.**<br>
*Satoshi Murai, Meng-Yu Jennifer Kuo, Ryo Kawahara, Shohei Nobuhara, Ko Nishino.*<br> 
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Murai_Surface_Normals_and_Shape_From_Water_ICCV_2019_paper.pdf)]

**Surface Normals in the Wild.**<br>
*Weifeng Chen, Donglai Xiang, Jia Deng.*<br>
ICCV 2017, Invited Poster at the Bridges to 3D Workshop, CVPR 2018.
[[PDF](https://arxiv.org/abs/1704.02956)] [[Dataset](http://www-personal.umich.edu/~wfchen/surface-normals-in-the-wild/)] [[Gihtub](https://github.com/princeton-vl/surface_normals)]

### Scene Reconstruction

**Unsupervised Monocular Depth Reconstruction of Non-Rigid Scenes.**<br>
*Ayça Takmaz, Danda Pani Paudel, Thomas Probst, Ajad Chhatkuli, Martin R. Oswald, Luc Van Gool.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2012.15680)]

**Multi-layer Depth and Epipolar Feature Transformers for 3D Scene Reconstruction.**<br>
*Daeyun Shin, Zhile Ren, Erik B. Sudderth, Charless C. Fowlkes.*<br>
CVPR 2019. [[PDF](http://openaccess.thecvf.com/content_CVPRW_2019/papers/SUMO/Shin_Multi-layer_Depth_and_Epipolar_Feature_Transformers_for_3D_Scene_Reconstruction_CVPRW_2019_paper.pdf)]

**Image-to-Voxel Model Translation for 3D Scene Reconstruction and Segmentation.**<br>
*Vladimir V. Kniaz, Vladimir A. Knyaz, Fabio Remondino, Artem Bordodymov, Petr Moshkantsev.*<br> 
ECCV 2020. [[pdf](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123520103.pdf)] [[Supplement](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123520103-supp.zip)]

**FlatNet: Towards Photorealistic Scene Reconstruction from Lensless Measurements.**<br>
*Salman S. Khan, Varun Sundar, Vivek Boominathan, Ashok Veeraraghavan, Kaushik Mitra.*<br>
TPAMI 2020. [[PDF](https://arxiv.org/abs/2010.15440)] [[Project](https://siddiquesalman.github.io/flatnet/)]

**Learning to Recover 3D Scene Shape from a Single Image.**<br>
*Wei Yin, Jianming Zhang, Oliver Wang, Simon Niklaus, Long Mai, Simon Chen, Chunhua Shen.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.09365)]

### General Object Reconstruction

**DI-Fusion: Online Implicit 3D Reconstruction with Deep Priors.**<br>
*Jiahui Huang, Shi-Sheng Huang, Haoxuan Song, Shi-Min Hu.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.05551)]

**Compositionally Generalizable 3D Structure Prediction.**<br>
*Songfang Han, Jiayuan Gu, Kaichun Mo, Li Yi, Siyu Hu, Xuejin Chen, Hao Su.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.02493)]

**STaR: Self-supervised Tracking and Reconstruction of Rigid Objects in Motion with Neural Rendering.**<br>
*Wentao Yuan, Zhaoyang Lv, Tanner Schmidt, Steven Lovegrove.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2101.01602)]

**Descriptor-Free Multi-View Region Matching for Instance-Wise 3D Reconstruction.**<br>
*Takuma Doi, Fumio Okura, Toshiki Nagahara, Yasuyuki Matsushita, Yasushi Yagi.*<br>
ACCV 2020. [[PDF](https://arxiv.org/abs/2011.13649)]

**Deep Optimized Priors for 3D Shape Modeling and Reconstruction.**<br>
*Mingyue Yang, Yuxin Wen, Weikai Chen, Yongwei Chen, Kui Jia.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.07241)]

**VMR: Online Adaptation for Consistent Mesh Reconstruction in the Wild.**<br>
*Xueting Li, Sifei Liu, Shalini De Mello, Kihwan Kim, Xiaolong Wang, Ming-Hsuan Yang, Jan Kautz.*<br>
NeurIPS 2020. [[PDF](https://sites.google.com/nvidia.com/vmr-2020)]

**A Divide et Impera Approach for 3D Shape Reconstruction from Multiple Views.**<br>
*Riccardo Spezialetti, David Joseph Tan, Alessio Tonioni, Keisuke Tateno, Federico Tombari.*<br>
3DV 2020. [[PDF](https://arxiv.org/abs/2011.08534)]

**Learning Canonical Transformations.**<br>
*Zachary Dulberg, Jonathan Cohen.*<br>
NeurIPS 2020 Workshop on BabyMind. [[PDF](https://arxiv.org/abs/2011.08822)]

**Adversarial Generation of Continuous Implicit Shape Representations.**<br>
*Marian Kleineberg, Matthias Fey, Frank Weichert.*<br>
Eurographics 2020. [[PDF](https://arxiv.org/abs/2002.00349)] [[Github](https://github.com/marian42/shapegan)]

**Convolutional Generation of Textured 3D Meshes.**<br>
*Dario Pavllo, Graham Spinks, Thomas Hofmann, Marie-Francine Moens, and Aurelien Lucchi.*<br>
NeurIPS 2020. [[PDF](https://arxiv.org/abs/2006.07660)] [[Github](https://github.com/dariopavllo/convmesh)]

**Learning Deformable Tetrahedral Meshes for 3D Reconstruction.**<br>
*Jun Gao, Wenzheng Chen, Tommy Xiang, Alec Jacobson, Morgan McGuire, Sanja Fidler.*<br>
NeurIPS 2020. [[PDF](https://arxiv.org/abs/2011.01437)]

**Primal-Dual Mesh Convolutional Neural Networks.**<br>
*Francesco Milano, Antonio Loquercio, Antoni Rosinol, Davide Scaramuzza, Luca Carlone.*<br>
NeurIPS 2020. [[PDF](https://arxiv.org/abs/2010.12455)] [[Github](https://github.com/MIT-SPARK/PD-MeshNet)]

**Neural Star Domain as Primitive Representation.**<br>
*Yuki Kawana, Yusuke Mukuta, Tatsuya Harada.*<br>
NeurIPS 2020. [[PDF](https://arxiv.org/abs/2010.11248)]

**SDF-SRN: Learning Signed Distance 3D Object Reconstruction from Static Images.**<br>
*Chen-Hsuan Lin, Chaoyang Wang, Simon Lucey.*<br>
NeurIPS 2020. [[PDF](https://arxiv.org/abs/2010.10505)] [[Github](https://chenhsuanlin.bitbucket.io/signed-distance-SRN/)]

**PlaneRCNN: 3D Plane Detection and Reconstruction from a Single Image.**<br>
*[Chen Liu](http://art-programmer.github.io/), [Kihwan Kim](https://research.nvidia.com/person/kihwan-kim), [Jinwei Gu](http://www.gujinwei.org/), [Yasutaka Furukawa](http://www.cs.sfu.ca/~furukawa/), [Jan Kautz](https://research.nvidia.com/person/jan-kautz).*<br>
CVPR 2019. [[PDF](https://arxiv.org/pdf/1812.04072.pdf)] [[Github](https://github.com/NVlabs/planercnn)] [[Project](https://research.nvidia.com/publication/2019-06_PlaneRCNN)]

**Monocular Differentiable Rendering for Self-Supervised 3D Object Detection.**<br>
*Deniz Beker, Hiroharu Kato, Mihai Adrian Morariu, Takahiro Ando, Toru Matsuoka, Wadim Kehl, Adrien Gaidon.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2009.14524)]

**UMR: Self-supervised Single-view 3D Reconstruction via Semantic Consistency.**<br>
*[Xueting Li](https://sunshineatnoon.github.io/), [Sifei Liu](https://www.sifeiliu.net/), Kihwan Kim, Shalini De Mello, Varun Jampani, Ming-Hsuan Yang, Jan Kautz.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2003.06473)] [[Project](https://sites.google.com/nvidia.com/unsup-mesh-2020)] [[Github](https://github.com/NVlabs/UMR)]

**Learning Gradient Fields for Shape Generation.**<br>
*Ruojin Cai, Guandao Yang, Hadar Averbuch-Elor, Zekun Hao, Serge Belongie, Noah Snavely, Bharath Hariharan.*<br>
ECCV 2020. [[pdf](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123480375.pdf)] [[Supplement](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123480375-supp.pdf)]

**Who Left the Dogs Out? 3D Animal Reconstruction with Expectation Maximization in the Loop.**<br> 
*Benjamin Biggs, Oliver Boyne, James Charles, Andrew Fitzgibbon, Roberto Cipolla.*<br>
ECCV 2020. [[pdf](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123560188.pdf)] [[Supplement](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123560188-supp.zip)]

**MRGAN: Multi-Rooted 3D Shape Generation with Unsupervised Part Disentanglement.**<br>
*Rinon Gal, Amit Bermano, Hao Zhang, Daniel Cohen-Or.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2007.12944)]

**Mask2CAD: 3D Shape Prediction by Learning to Segment and Retrieve.**<br>
*Weicheng Kuo, Anelia Angelova, Tsung-Yi Lin, Angela Dai.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.13034)]

**Associative3D: Volumetric Reconstruction from Sparse Views.**<br>
*Shengyi Qian, Linyi Jin, David F. Fouhey.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.13727)] [[Github](https://jasonqsy.github.io/Associative3D)]

**Front2Back: Single View 3D Shape Reconstruction via Front to Back Prediction.**<br>
*Yuan Yao, Nico Schertler, Enrique Rosales, Helge Rhodin, Leonid Sigal, Alla Sheffer.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/1912.10589)]

**Pix2Vox++: Multi-scale Context-aware 3D Object Reconstruction from Single and Multiple Images.**<br>
*Haozhe Xie, Hongxun Yao, Shengping Zhang, Shangchen Zhou, Wenxiu Sun.*<br>
IJCV 2020. [[PDF](https://arxiv.org/abs/2006.12250)]

**Learning Generative Models of Shape Handles.**<br>
*Matheus Gadelha, Giorgio Gori, Duygu Ceylan, Radomir Mech, Nathan Carr, Tamy Boubekeur, Rui Wang, Subhransu Maji.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.03028)]

**Learning to Detect 3D Reflection Symmetry for Single-View Reconstruction.**<br>
*Yichao Zhou, Shichen Liu, Yi Ma.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2006.10042)]

**DOPS: Learning to Detect 3D Objects and Predict their 3D Shapes.**<br>
*Mahyar Najibi, Guangda Lai, Abhijit Kundu, Zhichao Lu, Vivek Rathod, Tom Funkhouser, Caroline Pantofaru, David Ross, Larry S. Davis, Alireza Fathi.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.01170)]

**Modeling 3D Shapes by Reinforcement Learning.**<br>
*Cheng Lin, Tingxiang Fan, Wenping Wang, Matthias Nießner.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2003.12397)]

**SymmetryNet: Learning to Predict Reflectional and Rotational Symmetries of 3D Shapes from Single-View RGB-D Images.**<br>
*Yifei Shi, Junwen Huang, Hongjia Zhang, Xin Xu, Szymon Rusinkiewicz, Kai Xu.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.00485)]

**Unsupervised Learning of Probably Symmetric Deformable 3D Objects from Images in the Wild.**<br>
*[Shangzhe Wu](https://elliottwu.com/), Christian Rupprecht, Andrea Vedaldi.*<br>
CVPR 2020 Best Paper. [[PDF](https://arxiv.org/abs/1911.11130)] [[Project](https://elliottwu.com/projects/unsup3d/)]

**GAN2Shape: Do 2D GANs Know 3D Shape? Unsupervised 3D shape reconstruction from 2D Image GANs.**<br>
*Xingang Pan, Bo Dai, Ziwei Liu, Chen Change Loy, Ping Luo.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.00844)] [[Github](https://github.com/XingangPan/GAN2Shape)] [[Project](https://xingangpan.github.io/projects/GAN2Shape.html)]

**Self-supervised Single-view 3D Reconstruction via Semantic Consistency.**<br>
*Xueting Li, Sifei Liu, Kihwan Kim, Shalini De Mello, Varun Jampani, Ming-Hsuan Yang, Jan Kautz.*<br>
arxiv, 13 Mar 2020. [[PDF](https://arxiv.org/abs/2003.06473)] [[Project](https://sites.google.com/view/unsup-mesh/home)]

**Inverse Graphics GAN: Learning to Generate 3D Shapes from Unstructured 2D Data.**<br>
*Sebastian Lunz, Yingzhen Li, Andrew Fitzgibbon, Nate Kushman.*<br>
arxiv, 28 Feb 2020. [[PDF](https://arxiv.org/abs/2002.12674)]

**SDFDiff: Differentiable Rendering of Signed Distance Fields for 3D Shape Optimization.**<br>
*Yue Jiang, Dantong Ji, Zhizhong Han, Matthias Zwicker.*<br>
arxiv, 15 Dec 2019. [[PDF](https://arxiv.org/abs/1912.07109)]

**Learning to Reconstruct 3D Manhattan Wireframes from a Single Image.**<br>
*Yichao Zhou, [Haozhi Qi](https://people.eecs.berkeley.edu/~hqi/), Yuexiang Zhai, Qi Sun, Zhili Chen, [Li-Yi Wei](https://research.adobe.com/person/li-yi-wei/), [Yi Ma](https://people.eecs.berkeley.edu/~yima/).*<br>
ICCV 2019. [[PDF](https://people.eecs.berkeley.edu/~hqi/)] [[Video Demonstration](https://youtu.be/l3sUtddPJPY)]

**Facial Details Synthesis From Single Input Image.**<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1903.10873)] [[Supplemental Material](https://github.com/apchenstu/Facial_Details_Synthesis/blob/master/src/imgs/Supplemental_Material.pdf)] [[Github](https://github.com/apchenstu/Facial_Details_Synthesis)]

**Photo-Realistic Facial Details Synthesis from Single Image.**<br>
*Anpei Chen, Zhang Chen, Guli Zhang, Ziheng Zhang, Kenny Mitchell, Jingyi Yu.*<br> 
ICCV 2019. [[PDF](https://arxiv.org/abs/1903.10873)] [[Supplemental Material](https://github.com/apchenstu/Facial_Details_Synthesis/blob/master/src/imgs/Supplemental_Material.pdf)] [[Github](https://github.com/apchenstu/Facial_Details_Synthesis)]

**Unsupervised 3D Reconstruction Networks.**<br>
*Geonho Cha, Minsik Lee, Songhwai Oh.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Cha_Unsupervised_3D_Reconstruction_Networks_ICCV_2019_paper.pdf)]

**Domain-Adaptive Single-View 3D Reconstruction.**<br>
*Pedro O. Pinheiro, Negar Rostamzadeh, Sungjin Ahn.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Pinheiro_Domain-Adaptive_Single-View_3D_Reconstruction_ICCV_2019_paper.pdf)]

**Neural 3D Mesh Renderer.**<br>
*Hiroharu Kato, Yoshitaka Ushiku, Tatsuya Harada.*<br>
CVPR 2018. [[PDF](https://arxiv.org/abs/1711.07566)] [[Project](http://hiroharu-kato.com/projects_en/neural_renderer.html)] [[Github](https://github.com/hiroharu-kato/neural_renderer)]

### Object Skeletonization

**Image Co-skeletonization via Co-segmentation.**<br>
*Koteswar Rao Jerripothula, Jianfei Cai, Jiangbo Lu, Junsong Yuan.*<br>
TIP 2020. [[PDF](https://arxiv.org/abs/2004.05575)]

### Shape and Viewpoint

**Novel Object Viewpoint Estimation through Reconstruction Alignment.**<br>
*Mohamed El Banani, Jason J. Corso, David F. Fouhey.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2006.03586)] [[Project](https://mbanani.github.io/novelviewpoints/)]

**Self-supervised 3D Shape and Viewpoint Estimation from Single Images for Robotics.**<br>
*Oier Mees, Maxim Tatarchenko, Thomas Brox and Wolfram Burgard.*<br>
IROS 2019. [[PDF](https://arxiv.org/abs/1910.07948.pdf)]

**Self-Supervised Viewpoint Learning From Image Collections.**<br>
*Siva Karthik Mustikovela, Varun Jampani, Shalini De Mello, Sifei Liu, Umar Iqbal, Carsten Rother, Jan Kautz.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.01793)]

## Pose Estimation

[[Awesome work on hand pose estimation/tracking.](https://github.com/xinghaochen/awesome-hand-pose-estimation)]

**Camera-to-Robot Pose Estimation from a Single Image.**<br>
*Timothy E. Lee, Jonathan Tremblay, Thang To, Jia Cheng, Terry Mosier, Oliver Kroemer, Dieter Fox, Stan Birchfield.*<br>
[[PDF](https://arxiv.org/abs/1911.09231)]

**Mask-pose Cascaded CNN for 2D Hand Pose Estimation from Single Color Images.**<br>
**Yangang Wang, Cong Peng, Yebin Liu.**<br>
IEEE Trans. CSVT 2019. [[Project](https://www.yangangwang.com/papers/WANG-MCC-2018-10.html)]
[[PDF](http://www.liuyebin.com/hand2d/hand2d.pdf)] 

**RGBD-Dog: Predicting Canine Pose from RGBD Sensors.**
*Sinead Kearney, Wenbin Li, Martin Parsons, Kwang In Kim, Darren Cosker.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.07788)]

## Depth Estimation

### Dynamic Object

**HDNet: Human Depth Estimation for Multi-Person Camera-Space Localization.**<br>
*Jiahao Lin, Gim Hee Lee.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.08943)]

**Self-Supervised Monocular Depth Estimation: Solving the Dynamic Object Problem by Semantic Guidance.**<br>
*Marvin Klingner, Jan-Aike Termöhlen, Jonas Mikolajczyk, Tim Fingscheidt.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.06936)]

### Accurate Edge

**P2ORM: Pixel-Pair Occlusion Relationship Map(P2ORM): Formulation, Inference & Application.**<br>
*Xuchong Qiu, Yang Xiao, Chaohui Wang, Renaud Marlet.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.12088)] [[Project](http://imagine.enpc.fr/~qiux/P2ORM/)] [[Github](https://github.com/tim885/P2ORM)]

**Semantics-Driven Unsupervised Learning for Monocular Depth and Ego-Motion Estimation.**<br>
*Xiaobin Wei, Jianjiang Feng, Jie Zhou.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2006.04371)]

**DispFields: Predicting Sharp and Accurate Occlusion Boundaries in Monocular Depth Estimation Using Displacement Fields.**<br>
*[Michael Ramamonjisoa](https://michaelramamonjisoa.github.io/), Yuming Du, Vincent Lepetit.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2002.12730)]
[[Github](https://github.com/dulucas/DisplacementFields)] [[Project](https://michaelramamonjisoa.github.io/projects/DisplacementFields)]

**SharpNet: Fast and Accurate Recovery of Occluding Contours in Monocular Depth Estimation.**<br>
*Michael Ramamonjisoa, Vincent Lepetit.*<br>
ICCV Workshops 2019. [[PDF](http://openaccess.thecvf.com/content_ICCVW_2019/papers/3DRW/Ramamonjisoa_SharpNet_Fast_and_Accurate_Recovery_of_Occluding_Contours_in_Monocular_ICCVW_2019_paper)] [[Github](https://github.com/MichaelRamamonjisoa/SharpNet)]

**EdgeDepth: The Edge of Depth: Explicit Constraints between Segmentation and Depth.**<br>
*[Shengjie Zhu](http://cvlab.cse.msu.edu/author/shengjie-zhu.html), Garrick Brazil and Xiaoming Liu.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.00171)] [[Github](https://github.com/TWJianNuo/EdgeDepth-Release)] [[Project](http://cvlab.cse.msu.edu/project-edgedepth.html)]

**Structure-Aware Residual Pyramid Network for Monocular Depth Estimation.**<br>
*Xiaotian Chen, Xuejin Chen, and Zheng-Jun Zha.*<br>
IJCAI 2019. [[PDF](https://arxiv.org/abs/1907.06023)] [[Github](https://github.com/Xt-Chen/SARPN)]

**Revisiting Single Image Depth Estimation: Toward Higher Resolution Maps with Accurate Object Boundaries.**<br>
*Junjie Hu, Mete Ozay, Yan Zhang, Takayuki Okatani.*<br>
WACV 2019. [[PDF](https://arxiv.org/abs/1803.08673)] [[Github](https://github.com/JunjH/Revisiting_Single_Depth_Estimation)] [[Data](https://drive.google.com/file/d/1WoOZOBpOWfmwe7bknWS5PMUCLBPFKTOw/view?usp=sharing)]

### Depth From Video (Depth, Normal and Camera Motion Estimation)

**DeepVideoMVS: Multi-View Stereo on Video with Recurrent Spatio-Temporal Fusion.**<br>
*Arda Düzçeker, Silvano Galliani, Christoph Vogel, Pablo Speciale, Mihai Dusmanu, Marc Pollefeys.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.02177)] [[Github](https://github.com/ardaduz/deep-video-mvs)]

**Consistent Video Depth Estimation.**<br>
*Xuan Luo, Jia-Bin Huang, Richard Szeliski, Kevin Matzen, Johannes Kopf.*<br>
SIGGRAPH 2020. [[PDF](https://arxiv.org/abs/2004.15021)] [[Project](https://roxanneluo.github.io/Consistent-Video-Depth-Estimation/)]

**Self-supervised Object Motion and Depth Estimation from Video.**<br>
*Qi Dai, Vaishakh Patil, Simon Hecker, Dengxin Dai, Luc Van Gool, Konrad Schindler.*<br>
arxiv, Dec 2019. [[PDF](https://arxiv.org/abs/1912.04250)]

**DeepFactors: Real-Time Probabilistic Dense Monocular SLAM.**<br>
*Jan Czarnowski, Tristan Laidlow, Ronald Clark, Andrew J. Davison.*<br>
arxiv, 14 Jan 2020. [[PDF](https://arxiv.org/abs/2001.05049)] [[Github](https://github.com/jczarnowski/DeepFactors)]

**DIODE: A Dense Indoor and Outdoor DEpth Dataset.**<br>
*Igor Vasiljevic, Nick Kolkin, Shanyi Zhang, Ruotian Luo, Haochen Wang, Falcon Z. Dai, Andrea F. Daniele, Mohammadreza Mostajabi, Steven Basart, Matthew R. Walter, Gregory Shakhnarovich.*<br>
CVPR 2020. 
[[PDF](arxiv.org/pdf/1908.00463.pdf)]
[[Project](diode-dataset.org)] 
[[Github](github.com/diode-dataset/)]
[[Frontiers of Monocular 3D Perception | Workshop CVPR 2020 ](https://sites.google.com/view/mono3d-workshop/home)]

**Joint Graph-based Depth Refinement and Normal Estimation.**<br>
*Mattia Rossi, Mireille El Gheche, Andreas Kuhn, Pascal Frossard.*<br>
arxiv, 3 Dec 2019. [[PDF](https://arxiv.org/abs/1912.01306)]

**Monocular Neural Image Based Rendering With Continuous View Control.**<br>
*Xu Chen, Jie Song, Otmar Hilliges.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Chen_Monocular_Neural_Image_Based_Rendering_With_Continuous_View_Control_ICCV_2019_paper.pdf)]

**Self-Supervised Monocular Depth Hints.**<br>
*Jamie Watson, Michael Firman, Gabriel J. Brostow, Daniyar Turmukhambetov.*<br> 
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Watson_Self-Supervised_Monocular_Depth_Hints_ICCV_2019_paper.pdf)]

**Object-Specific Distance From a Monocular Image.**<br>
*Jing Zhu, Yi Fang.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Zhu_Learning_Object-Specific_Distance_From_a_Monocular_Image_ICCV_2019_paper.pdf)]

**Depth From Videos in the Wild: Unsupervised Monocular Depth Learning From Unknown Cameras.**<br>
*Ariel Gordon, Hanhan Li, Rico Jonschkowski, Anelia Angelova.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Gordon_Depth_From_Videos_in_the_Wild_Unsupervised_Monocular_Depth_Learning_ICCV_2019_paper.pdf)] [[Github](https://github.com/google-research/google-research/tree/master/depth_from_video_in_the_wild)]

**Towards Robust Monocular Depth Estimation: Mixing Datasets for Zero-Shot Cross-Dataset Transfer.**<br>
*Katrin Lasinger, René Ranftl, Konrad Schindler, Vladlen Koltun.*<br>
[[PDF](https://arxiv.org/abs/1907.01341)]

**SynDeMo: Synergistic Deep Feature Alignment for Joint Learning of Depth and Ego-Motion.**<br>
*Behzad Bozorgtabar, Mohammad Saeed Rad, Dwarikanath Mahapatra, Jean-Philippe Thiran.*<br> 
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Bozorgtabar_SynDeMo_Synergistic_Deep_Feature_Alignment_for_Joint_Learning_of_Depth_ICCV_2019_paper.pdf)]

**Insta-DM: Instance-wise Depth and Motion Learning from Monocular Videos.**<br>
*Seokju Lee, Sunghoon Im, Stephen Lin, In So Kweon.*<br>
arxiv, 19 Dec 2019.
[[PDF](https://arxiv.org/abs/1912.09351)] 
[[Project](http://sites.google.com/site/seokjucv/home/instadm)] 
[[Github](https://github.com/SeokjuLee/Insta-DM)]

**Self-Supervised Learning With Geometric Constraints in Monocular Video: Connecting Flow, Depth, and Camera.**<br>
*Yuhua Chen, Cordelia Schmid, Cristian Sminchisescu.*<br> 
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Chen_Self-Supervised_Learning_With_Geometric_Constraints_in_Monocular_Video_Connecting_Flow_ICCV_2019_paper.pdf)]

**Spatial Correspondence With Generative Adversarial Network: Learning Depth From Monocular Videos.**<br>
*Zhenyao Wu, Xinyi Wu, Xiaoping Zhang, Song Wang, Lili Ju.*<br> 
ICCV 2019. [[PDF](http://openaccess.thecvf.com/ICCV2019.py#)]

**Deep Optics for Monocular Depth Estimation and 3D Object Detection.**<br>
*Julie Chang, Gordon Wetzstein.*<br> 
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Chang_Deep_Optics_for_Monocular_Depth_Estimation_and_3D_Object_Detection_ICCV_2019_paper.pdf)]

**Learning Single Camera Depth Estimation Using Dual-Pixels.**<br>
*Rahul Garg, Neal Wadhwa, Sameer Ansari, Jonathan T. Barron.*<br> 
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Garg_Learning_Single_Camera_Depth_Estimation_Using_Dual-Pixels_ICCV_2019_paper.pdf)]

**Enforcing Geometric Constraints of Virtual Normal for Depth Prediction.**<br>
*Wei Yin, Yifan Liu, Chunhua Shen, Youliang Yan.*<br> 
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Yin_Enforcing_Geometric_Constraints_of_Virtual_Normal_for_Depth_Prediction_ICCV_2019_paper.pdf)]

**Exploiting Temporal Consistency for Real-Time Video Depth Estimation.**<br>
*Haokui Zhang, Chunhua Shen, Ying Li, Yuanzhouhan Cao, Yu Liu, Youliang Yan.*<br> 
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Zhang_Exploiting_Temporal_Consistency_for_Real-Time_Video_Depth_Estimation_ICCV_2019_paper.pdf)]

**Moving Indoor: Unsupervised Video Depth Learning in Challenging Environments.**<br>
*Junsheng Zhou, Yuwang Wang, Kaihuai Qin, Wenjun Zeng.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Zhou_Moving_Indoor_Unsupervised_Video_Depth_Learning_in_Challenging_Environments_ICCV_2019_paper.pdf)]

**The Sound of Motions.**<br>
*Hang Zhao, Chuang Gan, Wei-Chiu Ma, Antonio Torralba.*<br> 
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Jo_SC-FEGAN_Face_Editing_Generative_Adversarial_Network_With_Users_Sketch_and_ICCV_2019_paper.pdf)]

**Self-Supervised Monocular Depth Hints.**<br>
*Jamie Watson, Michael Firman, Gabriel J. Brostow, Daniyar Turmukhambetov.*<br> 
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Watson_Self-Supervised_Monocular_Depth_Hints_ICCV_2019_paper.pdf)]

**Monocular Piecewise Depth Estimation in Dynamic Scenes by Exploiting Superpixel Relations.**<br>
*Yan Di, Henrique Morimitsu, Shan Gao, Xiangyang Ji.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Di_Monocular_Piecewise_Depth_Estimation_in_Dynamic_Scenes_by_Exploiting_Superpixel_ICCV_2019_paper.pdf)]

**How Do Neural Networks See Depth in Single Images?**<br>
*Tom van Dijk, Guido de Croon.*<br> 
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/van_Dijk_How_Do_Neural_Networks_See_Depth_in_Single_Images_ICCV_2019_paper.pdf)]

**On Boosting Single-Frame 3D Human Pose Estimation via Monocular Videos.**<br> 
*Zhi Li, Xuan Wang, Fei Wang, Peilin Jiang.*<br>
ICCV 2019.[[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Li_On_Boosting_Single-Frame_3D_Human_Pose_Estimation_via_Monocular_Videos_ICCV_2019_paper.pdf)]

**Canonical Surface Mapping via Geometric Cycle Consistency.**<br>
*Nilesh Kulkarni, Abhinav Gupta, Shubham Tulsiani.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Kulkarni_Canonical_Surface_Mapping_via_Geometric_Cycle_Consistency_ICCV_2019_paper.pdf)]

**Mono-SF: Multi-View Geometry Meets Single-View Depth for Monocular Scene Flow Estimation of Dynamic Traffic Scenes.**<br>
*Fabian Brickwedde, Steffen Abraham, Rudolf Mester.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Brickwedde_Mono-SF_Multi-View_Geometry_Meets_Single-View_Depth_for_Monocular_Scene_Flow_ICCV_2019_paper.pdf)]

**Digging Into Self-Supervised Monocular Depth Estimation.**<br>
*Clement Godard, Oisin Mac Aodha, Michael Firman, Gabriel J. Brostow.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Godard_Digging_Into_Self-Supervised_Monocular_Depth_Estimation_ICCV_2019_paper.pdf)]

**Learning the Depths of Moving People by Watching Frozen People.**<br>
*Zhengqi Li, Tali Dekel, Forrester Cole, Richard Tucker, Noah Snavely, Ce Liu, William T. Freeman.*<br>
CVPR 2019 (oral). [[PDF](https://arxiv.org/abs/1904.11111)] [[Project](https://mannequin-depth.github.io/)]

**Learning Single-Image Depth from Videos using Quality Assessment Networks.**<br>
*[Weifeng Chen](http://www-personal.umich.edu/~wfchen/), Shengyi Qian, Jia Deng.*<br>  
CVPR 2019. [[PDF](https://arxiv.org/abs/1806.09573)] [[Project](http://www-personal.umich.edu/~wfchen/youtube3d/)] [Github](https://github.com/princeton-vl/YouTube3D)]

**Unsupervised Monocular Depth and Ego-motion Learning with Structure and Semantics.**<br>
*Vincent Casser, Soeren Pirk, Reza Mahjourian, Anelia Angelova.*<br>
CVPR Workshop on Visual Odometry & Computer Vision Applications Based on Location Clues (VOCVALC), 2019. [[PDF](https://arxiv.org/abs/1906.05717)]

**DFineNet: Ego-Motion Estimation and Depth Refinement from Sparse, Noisy Depth Input with RGB Guidance.**<br>
*Yilun Zhang, Ty Nguyen, Ian D. Miller, Shreyas S. Shivakumar, Steven Chen, Camillo J. Taylor, Vijay Kumar.*<br>
[[PDF](https://arxiv.org/abs/1903.06397)] [[Github](https://github.com/Ougui9/DFineNet)]

**Unsupervised Scale-consistent Depth and Ego-motion Learning from Monocular Video.**<br> 
*[Jia-Wang Bian](https://jwbian.net/), Zhichao Li, Naiyan Wang, Huangying Zhan, Chunhua Shen, Ming-Ming Cheng, Ian Reid.*<br>
NeurIPS 2019. [[Project](https://jwbian.net/sc-sfmlearner)] [[Github](https://github.com/JiawangBian/SC-SfMLearner-Release)] [[PDF](https://arxiv.org/abs/1908.10553)] 

**Beyond Photometric Loss for Self-Supervised Ego-Motion Estimation.**<br>
*Tianwei Shen, Zixin Luo, Lei Zhou, Hanyu Deng, Runze Zhang, Tian Fang, Long Quan.*<br> 
ICRA 2019. [[PDF](https://arxiv.org/abs/1902.09103)]

**Digging Into Self-Supervised Monocular Depth Estimation.**<br>
*[Clément Godard](http://www0.cs.ucl.ac.uk/staff/C.Godard/), Oisin Mac Aodha, Michael Firman, Gabriel Brostow.*<br> 
ICCV 2019. [[PDF](https://arxiv.org/abs/1806.01260)]

**Self-Supervised Learning of Depth and Motion Under Photometric Inconsistency.**<br>
*Tianwei Shen, Lei Zhou, Zixin Luo, Yao Yao, Shiwei Li, Jiahui Zhang, Tian Fang, Long Quan.*<br> 
ICCV Workshop 2019. [[PDF](https://arxiv.org/abs/1909.09115)]

**Depth Prediction Without the Sensors: Leveraging Structure for Unsupervised Learning from Monocular Videos.**<br>
*Vincent Casser, Soeren Pirk, Reza Mahjourian, Anelia Angelova.*<br> 
AAAI 2019. [[PDF](https://arxiv.org/abs/1811.06152)]

**GeoNet: Unsupervised Learning of Dense Depth, Optical Flow and Camera Pose.**<br>
*Zhichao Yin, Jianping Shi.*<br> 
CVPR 2018. [[PDF](https://arxiv.org/abs/1803.02276)] [[Github](https://github.com/yzcjtr/GeoNet)]

**Depth-VO-Feat: Unsupervised Learning of Monocular Depth Estimation and Visual Odometry with Deep Feature Reconstruction.**<br>
*Huangying Zhan, Ravi Garg, Chamara Saroj Weerasekera, Kejie Li, Harsh Agarwal, Ian Reid.*<br>
CVPR 2018.  [[PDF](https://arxiv.org/abs/1803.03893)] [[Github](https://github.com/Huangying-Zhan/Depth-VO-Feat)]

**LKVOLearner: Learning Depth from Monocular Videos using Direct Methods.**<br>
*Chaoyang Wang, Jose Miguel Buenaposada, Rui Zhu, Simon Lucey.*<br> 
CVPR 2018. [[PDF](https://arxiv.org/abs/1712.00175)] [[Github](https://github.com/MightyChaos/LKVOLearner)]

**Unsupervised Learning of Depth and Ego-Motion from Monocular Video Using 3D Geometric Constraints.**<br>
*Reza Mahjourian, Martin Wicke, Anelia Angelova.*<br>
CVPR 2018. [[PDF](https://arxiv.org/pdf/1802.05522.pdf)] [[Project](https://sites.google.com/view/vid2depth)]

**Visualization of Convolutional Neural Networks for Monocular Depth Estimation.**<br>
*Junjie Hu, Yan Zhang, Takayuki Okatani.*<br>
[[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Hu_Visualization_of_Convolutional_Neural_Networks_for_Monocular_Depth_Estimation_ICCV_2019_paper.pdf)]

**DeMoN: Depth and Motion Network for Learning Monocular Stereo.**<br>
*Benjamin Ummenhofer, Huizhong Zhou, Jonas Uhrig, Nikolaus Mayer, Eddy Ilg, Alexey Dosovitskiy, Thomas Brox.*<br>
CVPR 2017. [[PDF](https://arxiv.org/abs/1612.02401)] [[Project](https://lmb.informatik.uni-freiburg.de/people/ummenhof/depthmotionnet/), [Github](https://github.com/lmb-freiburg/demon)] 

**Unsupervised Learning of Depth and Ego-Motion from Video.**<br>
*[Tinghui Zhou](https://people.eecs.berkeley.edu/~tinghuiz/), Matthew Brown, Noah Snavely, David G. Lowe.*<br>
CVPR 2017. [[PDF](https://people.eecs.berkeley.edu/~tinghuiz/projects/SfMLearner/cvpr17_sfm_final.pdf)] [[Project](https://people.eecs.berkeley.edu/~tinghuiz/projects/SfMLearner/)] 

**MonoDepth: Unsupervised Monocular Depth Estimation with Left-Right Consistency.**<br>
*Clément Godard, Oisin Mac Aodha and Gabriel J. Brostow.*<br> 
CVPR 2017. [[PDF](https://arxiv.org/abs/1609.03677)] [[Project](http://visual.cs.ucl.ac.uk/pubs/monoDepth/)] [[Github](https://github.com/mrharicot/monodepth)]

**Learning from Synthetic Humans.**<br>
*Gül Varol, Javier Romero, Xavier Martin, Naureen Mahmood, Michael J. Black, Ivan Laptev, Cordelia Schmid.*<br>
CVPR 2017. [[PDF](https://arxiv.org/abs/1701.01370)] [[Project](http://www.di.ens.fr/willow/research/surreal)] [[Github](https://github.com/gulvarol/surreal)]

**Single-Image Depth Perception in the Wild.**<br>
*Weifeng Chen, Zhao Fu, Dawei Yang, Jia Deng.*<br>
NeurIPS 2016. [[PDF](https://arxiv.org/abs/1604.03901)] [[Dataset](http://www-personal.umich.edu/~wfchen/depth-in-the-wild/)] [[Github](https://github.com/princeton-vl/relative_depth)]

**Predicting Depth, Surface Normals and Semantic Labels with a Common Multi-Scale Convolutional Architecture.**<br>
*David Eigen, Rob Fergus.*<br>
ICCV 2015. [[PDF](https://arxiv.org/pdf/1411.4734v4.pdf)] [[Project](https://cs.nyu.edu/~deigen/dnl/)]

**Normal Estimation For "in-the-wild" Faces Using Fully Convolutional Networks.**<br>
*[Ｇ. Trigeorgis](http://trigeorgis.com), p. snape, S. Zafeiriou, I. Kokkinos.*<br>
CVPR 2017. [[PDF](https://ibug.doc.ic.ac.uk/media/uploads/documents/normalestimationcvpr2017_-4.pdf)] [[Supplementary](https://www.doc.ic.ac.uk/~gt108/papers/trigeorgis2017normals_supp.pdf)] [[Github](https://github.com/trigeorgis/face_normals_cvpr17)] 

### Depth with ToF

**Deep End-to-End Alignment and Refinement for Time-of-Flight RGB-D Module.**<br>
*Di Qiu, Jiahao Pang, [Wenxiu Sun](http://wenxiusun.com/), Chengxi Yang.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1909.07623)] [[Github](https://github.com/sylqiu/tof_rgbd_processing)]

**Deep End-to-End Time-of-Flight Imaging.**<br>
*Shuochen Su, Felix Heide, Gordon Wetzstein, Wolfgang Heidrich.*<br>
CVPR 2018. [[PDF](http://openaccess.thecvf.com/content_cvpr_2018/html/Su_Deep_End-to-End_Time-of-Flight_CVPR_2018_paper.html)] [[Github](https://github.com/shuochsu/DeepEnd2EndToFImaging)]

**Sparse-to-Dense: Depth Prediction from Sparse Depth Samples and a Single Image.**<br>
*[Fangchang Ma](http://www.mit.edu/~fcma), [Sertac Karaman](http://karaman.mit.edu/).*<br>
ICRA 2018. [[PDF](https://arxiv.org/abs/1709.07492)] [[Github](https://github.com/fangchangma/sparse-to-dense.pytorch)]

### Temporal- and Scale-Consistent Depth Estimation

**DeepVideoMVS: Multi-View Stereo on Video with Recurrent Spatio-Temporal Fusion.**<br>
*Arda Düzçeker, Silvano Galliani, Christoph Vogel, Pablo Speciale, Mihai Dusmanu, Marc Pollefeys.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.02177)] [[Github](https://github.com/ardaduz/deep-video-mvs)]

**TTNet: Real-Time Temporal and Spatial Video Analysis of Table Tennis.**<br>
*Roman Voeikov, Nikolay Falaleev, Ruslan Baikulov.*<br>
CVPR 2020 Workshop on Computer Vision in Sports (CVsports). [[PDF](https://arxiv.org/abs/2004.09927)]

**Predicting Sharp and Accurate Occlusion Boundaries in Monocular Depth Estimation Using Displacement Fields.**<br>
*Michael Ramamonjisoa, Yuming Du, Vincent Lepetit..*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2002.12730)]

**DiverseDepth: Affine-invariant Depth Prediction Using Diverse Data.**<br>
*Wei Yin, Xinlong Wang, Chunhua Shen, Yifan Liu, Zhi Tian, Songcen Xu, Changming Sun, Dou Renyin.*<br>
arxiv, 3 Feb 2020. [[PDF](https://arxiv.org/abs/2002.00569)]

**Towards Robust Monocular Depth Estimation: Mixing Datasets for Zero-shot Cross-dataset Transfer.**<br>
*René Ranftl, Katrin Lasinger, David Hafner, Konrad Schindler, Vladlen Koltun.*<br>
arxiv 2019. [[PDF](https://arxiv.org/abs/1907.01341)] [[Github](https://github.com/intel-isl/MiDaS)]

**Enforcing Geometric Constraints of Virtual Normal for Depth Prediction.**<br>
*Wei Yin, Yifan Liu, Chunhua Shen, Youliang Yan.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1907.12209)] [[Project](https://tinyurl.com/virtualnormal)]

**Neural RGB->D Sensing: Depth and Uncertainty from a Video Camera.**<br>
*[Chao Liu](http://www.cs.cmu.edu/~ILIM/people/chaoliu1/), [Jinwei Gu](http://www.gujinwei.org/), [Kihwan Kim](https://research.nvidia.com/person/kihwan-kim), Srinivasa Narasimhan, [Jan Kautz](https://research.nvidia.com/person/jan-kautz).*<br>
CVPR 2019. [[PDF](https://arxiv.org/abs/1901.02571)] [[Project](https://research.nvidia.com/publication/2019-06_Neural-RGBD)] [[Github](https://github.com/NVlabs/neuralrgbd)]

**Don't Forget The Past: Recurrent Depth Estimation from Monocular Video.**<br>
*Vaishakh Patil, Wouter Van Gansbeke, Dengxin Dai, Luc Van Gool.*<br>
arxiv, 8 Jan 2020. [[PDF](https://arxiv.org/abs/2001.02613)] [[Github](https://github.com/wvangansbeke/Recurrent-Depth-Estimation)]

**GLNet: Self-supervised Learning with Geometric Constraints in Monocular Video: Connecting Flow, Depth, and Camera.**<br>
*Yuhua Chen, Cordelia Schmid, Cristian Sminchisescu.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1907.05820)]

**Exploiting Temporal Consistency for Real-time Video Depth Estimation.**<br>
*Haokui Zhang, Chunhua Shen, Ying Li, Yuanzhouhan Cao, Yu Liu, Youliang Yan.*<br>
ICCV, 2019. [[PDF](https://arxiv.org/abs/1908.03706.pdf)] [[Project](https://tinyurl.com/STCLSTM)]

**Unsupervised Scale-consistent Depth and Ego-motion Learning from Monocular Video.**<br>
*Jia-Wang Bian, Zhichao Li, Naiyan Wang, Huangying Zhan, Chunhua Shen, Ming-Ming Cheng, Ian Reid.*<br>
NeurIPS, 2019.  
[[PDF](https://papers.nips.cc/paper/8299-unsupervised-scale-consistent-depth-and-ego-motion-learning-from-monocular-video.pdf)] 
[[Github](https://github.com/JiawangBian/SC-SfMLearner-Release)]
[[Project](https://jwbian.net/sc-sfmlearner)]

### Depth and Related Tasks

**Pattern-Affinitive Propagation Across Depth, Surface Normal and Semantic Segmentation.**<br>
*Zhenyu Zhang, Zhen Cui, Chunyan Xu, Yan Yan, Nicu Sebe, Jian Yang.*<br>
CVPR 2019. [[PDF](http://openaccess.thecvf.com/content_CVPR_2019/papers/Zhang_Pattern-Affinitive_Propagation_Across_Depth_Surface_Normal_and_Semantic_Segmentation_CVPR_2019_paper.pdf)]

**Competitive Collaboration: Joint Unsupervised Learning of Depth, Camera Motion, Optical Flow and Motion Segmentation.**<br>
*Anurag Ranjan, [Varun Jampani](https://varunjampani.github.io/), Lukas Balles, Kihwan Kim, Deqing Sun, Jonas Wulff, Michael J. Black.*<br>
CVPR 2019. 
[[PDF](http://openaccess.thecvf.com/content_CVPR_2019/papers/Ranjan_Competitive_Collaboration_Joint_Unsupervised_Learning_of_Depth_Camera_Motion_Optical_CVPR_2019_paper.pdf)]
[[Github](http://github.com/anuragranj/cc)]

## Learning Temporal Information from Videos
[Related Topics: Object Detection, Tracking and Segmentation.]

### FastSlow, Multiple Stream and Temporal Pyramid
**SlowFast Networks for Video Recognition.**<br>
*Christoph Feichtenhofer, Haoqi Fan, Jitendra Malik, Kaiming He.*<br>
ICCV 2019. 
[[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Feichtenhofer_SlowFast_Networks_for_Video_Recognition_ICCV_2019_paper.pdf)]
[[Github](https://github.com/facebookresearch/SlowFast)]

### 3D convolutions (C3D)
**Learning a Spatio-Temporal Embedding for Video Instance Segmentation.**<br>
*Anthony Hu, Alex Kendall, Roberto Cipolla.*<br>
ICLR 2020. [[PDF](https://arxiv.org/abs/1912.08969v1)]

**Fast Spatio-Temporal Residual Network for Video Super-Resolution.**<br>
*Sheng Li, Fengxiang He, Bo Du, Lefei Zhang, Yonghao Xu, Dacheng Tao.*<br>
CVPR 2019. [[PDF](http://openaccess.thecvf.com/content_CVPR_2019/papers/Li_Fast_Spatio-Temporal_Residual_Network_for_Video_Super-Resolution_CVPR_2019_paper.pdf)]

### Flow
**Unsupervised Scale-consistent Depth and Ego-motion Learning from Monocular Video.**<br>
*Jia-Wang Bian, Zhichao Li, Naiyan Wang, Huangying Zhan, Chunhua Shen, Ming-Ming Cheng, Ian Reid.*<br>
NeurIPS, 2019.  
[[PDF](https://papers.nips.cc/paper/8299-unsupervised-scale-consistent-depth-and-ego-motion-learning-from-monocular-video.pdf)] 
[[Github](https://github.com/JiawangBian/SC-SfMLearner-Release)]
[[Project](https://jwbian.net/sc-sfmlearner)]

### 2DCNN + LSTM (Temporal Block)
**Exploiting Temporal Consistency for Real-time Video Depth Estimation.**<br>
*Haokui Zhang, Chunhua Shen, Ying Li, Yuanzhouhan Cao, Yu Liu, Youliang Yan.*<br>
ICCV, 2019. [[PDF](https://arxiv.org/abs/1908.03706.pdf)] [[Project](https://tinyurl.com/STCLSTM)]

**3D Human Pose Estimation in Video with Temporal Convolutions and Semi-supervised Training.**<br>
*Dario Pavllo, Christoph Feichtenhofer, David Grangier, Michael Auli.*<br>
CVPR 2019. 
[[PDF](http://openaccess.thecvf.com/content_CVPR_2019/papers/Pavllo_3D_Human_Pose_Estimation_in_Video_With_Temporal_Convolutions_and_CVPR_2019_paper.pdf)] 
[[Github](https://github.com/facebookresearch/VideoPose3D)] [[Project](https://dariopavllo.github.io/VideoPose3D)]

## Misc (Speediness, Trajectories)

**Adversarial Generative Grammars for Human Activity Prediction.**<br>
*AJ Piergiovanni, Anelia Angelova, Alexander Toshev, Michael S. Ryoo.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2008.04888)]

**Long-term Human Motion Prediction with Scene Context.**<br>
*[Zhe Cao](http://people.eecs.berkeley.edu/~zhecao/), [Hang Gao](http://people.eecs.berkeley.edu/~hangg/), [Karttikeya Mangalam](https://karttikeya.github.io/), [Qi-Zhi Cai](https://scholar.google.com/citations?user=oyh-YNwAAAAJ&hl=en), [Minh Vo](https://minhpvo.github.io/), [Jitendra Malik](https://people.eecs.berkeley.edu/~malik/).*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.03672)] [[Github](https://github.com/ZheC/GTA-IM-Dataset)]

**MANTRA: Memory Augmented Networks for Multiple Trajectory Prediction.**<br>
*Francesco Marchetti, Federico Becattini, Lorenzo Seidenari, Alberto Del Bimbo.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2006.03340)]

**STINet: Spatio-Temporal-Interactive Network for Pedestrian Detection and Trajectory Prediction.**<br>
*Zhishuai Zhang, Jiyang Gao, Junhua Mao, Yukai Liu, Dragomir Anguelov, Congcong Li.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2005.04255)]

**SpeedNet: Learning the Speediness in Videos.**<br>
*[Sagie Benaim](https://sagiebenaim.github.io/), [Ariel Ephrat](http://www.cs.huji.ac.il/~arielephrat/), Oran Lang, Inbar Mosseri, [William T. Freeman](https://billf.mit.edu/), [Michael Rubinstein](http://people.csail.mit.edu/mrub/), [Michal Irani](http://www.weizmann.ac.il/math/irani/home), and [Tali Dekel](http://people.csail.mit.edu/talidekel/).*<br>
CVPR 2020. [[PDF](https://arxiv.org/pdf/2004.06130.pdf)] [[Project](https://speednet-cvpr20.github.io/)]

**Take a NAP: Non-Autoregressive Prediction for Pedestrian Trajectories.**<br>
*Hao Xue, Du. Q. Huynh, Mark Reynolds.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2004.09760)]

**TPNet: Trajectory Proposal Network for Motion Prediction.**<br>
*Liangji Fang, Qinhong Jiang, Jianping Shi, Bolei Zhou.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2004.12255)]


## Gaze Estimation, Tracking, Redirection, Correction, and Blink Detection

[[Awesome Work on Gaze Estimation.](https://github.com/cvlab-uob/Awesome-Gaze-Estimation)]

ICCV 2019 WorkShop: [Gaze Estimation and Prediction in the Wild](http://openaccess.thecvf.com/ICCV2019_workshops/ICCV2019_GAZE.py) [[Homepage](http://gazeworkshop.github.io/)]

* A Generalized and Robust Method Towards Practical Gaze Estimation on Smart Phone. [[PDF]](http://openaccess.thecvf.com/content_ICCVW_2019/papers/GAZE/Guo_A_Generalized_and_Robust_Method_Towards_Practical_Gaze_Estimation_on_ICCVW_2019_paper.pdf)
Tianchu Guo, Yongchao Liu, Hui Zhang, Xiabing Liu, Youngjun Kwak, Byung In Yoo, Jae-Joon Han, Changkyu Choi.

* Learning to Personalize in Appearance-Based Gaze Tracking. [[PDF]](http://openaccess.thecvf.com/content_ICCVW_2019/papers/GAZE/Linden_Learning_to_Personalize_in_Appearance-Based_Gaze_Tracking_ICCVW_2019_paper.pdf)
Erik Linden, Jonas Sjostrand, Alexandre Proutiere.

* On-Device Few-Shot Personalization for Real-Time Gaze Estimation. [[PDF]](http://openaccess.thecvf.com/content_ICCVW_2019/papers/GAZE/He_On-Device_Few-Shot_Personalization_for_Real-Time_Gaze_Estimation_ICCVW_2019_paper.pdf)
Junfeng He, Khoi Pham, Nachiappan Valliappan, Pingmei Xu, Chase Roberts, Dmitry Lagun, Vidhya Navalpakkam.

* RT-BENE: A Dataset and Baselines for Real-Time Blink Estimation in Natural Environments. [[PDF]](http://openaccess.thecvf.com/content_ICCVW_2019/papers/GAZE/Cortacero_RT-BENE_A_Dataset_and_Baselines_for_Real-Time_Blink_Estimation_in_ICCVW_2019_paper.pdf)
Kevin Cortacero, Tobias Fischer, Yiannis Demiris.

* SalGaze: Personalizing Gaze Estimation using Visual Saliency. [[PDF]](http://openaccess.thecvf.com/content_ICCVW_2019/papers/GAZE/Chang_SalGaze_Personalizing_Gaze_Estimation_using_Visual_Saliency_ICCVW_2019_paper.pdf)
Zhuoqing Chang, J. Matias Di Martino, Qiang Qiu, Steven Espinosa, Guillermo Sapiro.

### Gaze Dataset

**ETH-XGaze: A Large Scale Dataset for Gaze Estimation under Extreme Head Pose and Gaze Variation.**<br>
*Xucong Zhang, Seonwook Park, Thabo Beeler, Derek Bradley, Siyu Tang, Otmar Hilliges.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.15837)] [[ETH-XGaze](https://ait.ethz.ch/projects/2020/ETH-XGaze)]

**Columbia Gaze Data Set: Gaze Locking: Passive Eye Contact Detection for Human–Object Interaction.**<br>
*Brian A. Smith,  Qi Yin,  Steven K. Feiner,  Shree K. Nayar.*<br>
ACM Symposium on User Interface Software and Technology (UIST), 2013. [[PDF](http://www.cs.columbia.edu/~brian/publications/gaze_locking.html)] [[Columbia Gaze Data Set](http://www.cs.columbia.edu/CAVE/databases/columbia_gaze/)]

**GazeCapture: Eye Tracking for Everyone.**<br>
*Kyle Krafka*, Aditya Khosla*, Petr Kellnhofer, Harini Kannan, Suchendra Bhandarkar, Wojciech Matusik, Antonio Torralba.*<br>
CVPR 2016. [[PDF](https://gazecapture.csail.mit.edu/)] [[GazeCapture](https://gazecapture.csail.mit.edu/)] [[Github](https://github.com/CSAILVision/GazeCapture)]

**MPIIGaze: Appearance-based Gaze Estimation in the Wild.**<br>
*Xucong Zhang, Yusuke Sugano, Mario Fritz, Andreas Bulling.*<br>
CVPR 2015. [[PDF](https://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Zhang_Appearance-Based_Gaze_Estimation_2015_CVPR_paper.pdf)] [[MPIIGaze Dataset](https://www.mpi-inf.mpg.de/departments/computer-vision-and-machine-learning/research/gaze-based-human-computer-interaction/appearance-based-gaze-estimation-in-the-wild/)] [[Max Planck Institute for Informatics](www.mpi-inf.mpg.de/)]

**MPIIFaceGaze: It’s Written All Over Your Face: Full-Face Appearance-Based Gaze Estimation.**<br>
*X. Zhang, Y. Sugano, M. Fritz and A. Bulling.*<br>
CVPR Workshop, 2017. [[PDF]](https://perceptual.mpi-inf.mpg.de/files/2017/05/zhang_cvprw2017.pdf) [[Homepage]](https://www.mpi-inf.mpg.de/departments/computer-vision-and-machine-learning/research/gaze-based-human-computer-interaction/its-written-all-over-your-face-full-face-appearance-based-gaze-estimation/) [MPIIFaceGaze [Original](http://datasets.d2.mpi-inf.mpg.de/MPIIGaze/MPIIFaceGaze.zip) or [Normalized](http://datasets.d2.mpi-inf.mpg.de/MPIIGaze/MPIIFaceGaze_normalized.zip)]

**UT: Learning by Synthesis for Appearance-based 3D Gaze Estimation.**<br>
*Yusuke Sugano, Yasuyuki Matsushita, Yoichi Sato.*<br>
CVPR 2014. [[PDF](https://www.cv-foundation.org/openaccess/content_cvpr_2014/papers/Sugano_Learning-by-Synthesis_for_Appearance-based_2014_CVPR_paper.pdf)] [[UT Dataset](www.hci.iis.u-Tokyo.ac.jp/datasets)]

**Monocular Free-head 3D Gaze Tracking with Deep Learning and Geometry Constraints.**
*Haoping Deng, Wangjiang Zhu.*
ICCV 2017. [[PDF](http://openaccess.thecvf.com/content_ICCV_2017/papers/Zhu_Monocular_Free-Head_3D_ICCV_2017_paper.pdf)]

### Gaze Redirection and Correction

**Self-Learning Transformations for Improving Gaze and Head Redirection.**<br>
*Yufeng Zheng, Seonwook Park, Xucong Zhang, Shalini De Mello, Otmar Hilliges.*<br>
NeurIPS 2020. [[PDF](https://arxiv.org/abs/2010.12307)] [[Github](https://ait.ethz.ch/projects/2020/STED-gaze/)] [[Project](https://ait.ethz.ch/projects/2020/STED-gaze/)]

**MGGR: MultiModal-Guided Gaze Redirection with Coarse-to-Fine Learning.**<br> 
*Jingjing Chen, Jichao Zhang, Jiayuan Fan, Tao Chen, Enver Sangineto, Nicu Sebe.*<br> 
arxiv 2020. [[PDF](https://arxiv.org/abs/2004.03064)]

**GazeCorrection: Self-Guided Eye Manipulation in the wild using Self-Supervised Generative Adversarial Networks.**<br> 
*Jichao Zhang, Meng Sun, Jingjing Chen, Hao Tang, Yan Yan, Xueying Qin, Nicu Sebe.*<br> 
arxiv, 2019. [[PDF](https://arxiv.org/abs/1906.00805)] [[Github](https://github.com/zhangqianhui/GazeCorrection)]

**Look at Me! Correcting Eye Gaze in Live Video Communication.**<br> 
*Chih-Fan Hsu, Yushuen  Wang, C.-L Lei, Kuan-Ta Chen.*<br> 
TOMM (ACM Transactions on Multimedia Computing, Communications, and Applications). [[PDF](https://dl.acm.org/doi/10.1145/3311784)] [[Github](https://github.com/chihfanhsu/gaze_correction)]

**Photo-Realistic Monocular Gaze Redirection Using Generative Adversarial Networks.**<br>
*Zhe He, Adrian Spurr, Xucong Zhang, Otmar Hilliges ([AIT Lab, ETH Zurich](https://ait.ethz.ch/)).*<br> 
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/He_Photo-Realistic_Monocular_Gaze_Redirection_Using_Generative_Adversarial_Networks_ICCV_2019_paper.pdf)] [[Github](https://github.com/HzDmS/gaze_redirection)] [[Columbia Gaze Dataset](http://www.cs.columbia.edu/~brian/projects/columbia_gaze.html)] [[Processed](https://drive.google.com/file/d/1tE3QfFjxtRco4ruLZwYyUhjyYSp2QIJL/view?usp=sharing)]

**Improving Few-Shot User-Specific Gaze Adaptation via Gaze Redirection Synthesis.**<br>
*Yu Yu, Gang Liu, Jean-Marc Odobez.*<br>
CVPR 2019. [[PDF](http://www.idiap.ch/~odobez/publications/YuLiuOdobez-CVPR2019.pdf)]

**GazeDirector: Fully Articulated Eye Gaze Redirection in Video.**<br>
*Erroll Wood, Tadas Baltrusaitis, Louis-Philippe Morency, Peter Robinson, Andreas Bulling.*<br>
Eurographics 2018 (Best Paper Honourable Mention Award). [[PDF](https://perceptual.mpi-inf.mpg.de/files/2018/03/wood18_eg.pdf)] 

**GazeGAN: Unpaired Adversarial Image Generation for Gaze Estimation.**<br>
*Matan Sela, Pingmei Xu, Junfeng He, Vidhya Navalpakkam, Dmitry Lagun.*<br>
2017. [[PDF](https://arxiv.org/abs/1711.09767)]

**DeepWarp: Photorealistic Image Resynthesis for Gaze Manipulation.**<br>
*Yaroslav Ganin, Daniil Kononenko, Diana Sungatullina, Victor Lempitsky.*<br>
ECCV 2016. [[PDF](http://sites.skoltech.ru/compvision/projects/deepwarp/files/deepwarp_eccv2016.pdf)] [[Project](http://sites.skoltech.ru/compvision/projects/deepwarp/)]

**Learning to look up: Realtime Monocular Gaze Correction using Machine Learning.**<br>
CVPR 2015. [[PDF](https://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Kononenko_Learning_To_Look_2015_CVPR_paper.pdf)] 

**Gaze Correction for Home Video Conferencing.**<br>
*C. Kuster, T. Popa, J.C. Bazin, C. Gotsman, M. Gross.*<br>
ACM TOG 2012.  [[PDF](https://cgl.ethz.ch/disclaimer.php?dlurl=/Downloads/Publications/Papers/2012/Kus12/Kus12.pdf)] [[CGL ETHZ](https://cgl.ethz.ch/publications/papers/paperKus12.php)]

**An Eye For An Eye: A Single Camera Gaze-Replacement Method.**<br>
*[Lior Wolf](http://www.cs.tau.ac.il/~wolf/), Ziv Freund, Shai Avidan.*<br>
CVPR 2010. [[PDF](http://www.cs.tau.ac.il/~wolf/papers/eyes_cameraready.pdf)] 

**Eye Gaze Correction with Stereovision For Video-teleconferencing.**<br>
*Ruigang Yang, Zhengyou Zhang.*<br>
ECCV 2004. [[PDF](https://www.microsoft.com/en-us/research/publication/eye-gaze-correction-with-stereovision-for-video-teleconferencing/)]

### Gaze Estimation

**Learning to Detect Head Movement in Unconstrained Remote Gaze Estimation in the Wild.**<br>
*Zhecan Wang, Jian Zhao, Cheng Lu, Han Huang, Fan Yang, Lianji Li, Yandong Guo.*<br>
WACV 2020. [[PDF](https://arxiv.org/abs/2004.03737)]

**FAZE: Few-Shot Adaptive Gaze Estimation.**<br>
*Seonwook Park, Shalini De Mello, Pavlo Molchanov, Umar Iqbal, Otmar Hilliges, Jan Kautz.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Park_Few-Shot_Adaptive_Gaze_Estimation_ICCV_2019_paper.pdf)] [[Preprocess](github.com/swook/faze_preprocess)] [[Github](https://github.com/NVlabs/few_shot_gaze)] [[ETH Zurich](https://ait.ethz.ch/projects/2019/faze/)] [[Nvidia](https://research.nvidia.com/publication/2019-10_Few-Shot-Adaptive-Gaze)]

**Gaze360: Physically Unconstrained Gaze Estimation in the Wild.**<br>
*Petr Kellnhofer*, Adrià Recasens*, Simon Stent, Wojciech Matusik, Antonio Torralba.*<br>
ICCV 2019. [[PDF](http://gaze360.csail.mit.edu/iccv2019_gaze360.pdf)] [[Github](https://github.com/Erkil1452/gaze360)] [[Project](http://gaze360.csail.mit.edu)] [[Dataset](http://gaze360.csail.mit.edu/download.php)]

**Mixed Effects Neural Networks (MeNets) With Applications to Gaze Estimation.**<br>
*Yunyang Xiong, Hyunwoo J. Kim, Vikas Singh.*<br>
CVPR 2019. [[PDF](http://openaccess.thecvf.com/content_CVPR_2019/papers/Xiong_Mixed_Effects_Neural_Networks_MeNets_With_Applications_to_Gaze_Estimation_CVPR_2019_paper.pdf)]

**Deep Pictorial Gaze Estimation.**<br>
*Seonwook Park, Adrian Spurr, Otmar Hilliges.*<br>
ECCV 2018. [[PDF](http://openaccess.thecvf.com/content_ECCV_2018/papers/Seonwook_Park_Deep_Pictorial_Gaze_ECCV_2018_paper.pdf)] 

**RTGENE: Real-Time Gaze Estimation in Natural Environments.**<br>
*Tobias Fischer, Hyung Jin Chang,Yiannis Demiris.*<br>
ECCV 2018. [[PDF](http://openaccess.thecvf.com/content_ECCV_2018/papers/Tobias_Fischer_RT-GENE_Real-Time_Eye_ECCV_2018_paper.pdf)]
[[Github](https://github.com/Tobias-Fischer/rt_gene)]

### Eye Tracking

**EVE: Towards End-to-end Video-based Eye-Tracking.**<br>
*Seonwook Park, Emre Aksan, Xucong Zhang, Otmar Hilliges.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.13120)] [[Project](https://ait.ethz.ch/projects/2020/EVE)]

**Neuro-Inspired Eye Tracking With Eye Movement Dynamics.**<br>
*Kang Wang, Hui Su, Qiang Ji.*<br>
CVPR 2019. [[PDF](http://homepages.rpi.edu/~wangk10/papers/wang2019neural.pdf)]

**Generalizing Eye Tracking With Bayesian Adversarial Learning.**<br>
*Kang Wang, Rui Zhao, Hui Su, Qiang Ji.*<br>
CVPR 2019. [[PDF](https://www.semanticscholar.org/paper/Generalizing-Eye-Tracking-with-Bayesian-Adversarial-Wang-Zhao/77b9b6786699a236aad0c3fa3734730ece4a780f)]

**EyeDiap: A Database For the Development and Evaluation of Gaze Estimation Algorithms from RGB and RGBD Cameras.**<br>
*Kenneth Alberto Funes Mora, Florent Monay, Jeanmarc Odobez.*<br>
ETRA 2014. [[PDF](http://www.idiap.ch/~odobez/publications/FunesMonayOdobez-ETRA2014.pdf)] [[Idiap Research Institute](https://www.idiap.ch)]


## Team and People

[Real Virtual Humans](https://virtualhumans.mpi-inf.mpg.de), MPI-INF.

[Yebin Liu](http://www.liuyebin.com/), Associate Professor. 
Computational Photography and Reconstruction. 
Broadband Network & Digital Media Lab, Department of Automation, Tsinghua University, China.

[Gerard Pons-Moll](https://www.mpi-inf.mpg.de/departments/computer-vision-and-machine-learning/people/gerard-pons-moll/), 
Senior Researcher.
Max-Planck-Institut für Informatik, Germany.

[Thiemo Alldieck](https://graphics.tu-bs.de/people/alldieck), 
Researcher. 
Computer Graphics, TU Braunschweig, Germany.

## Good Start of 3D Resources (Python)

[Face3D](https://github.com/YadiraF/face3d). This project implements some basic functions related to 3D faces. You can use this to process mesh data, generate 3D faces from morphable model, reconstruct 3D face with a single image and key points as inputs, render faces with difference lightings.

[PySLAM](https://github.com/luigifreda/pyslam). pySLAM is a toy implementation of a monocular Visual Odometry (VO) pipeline in Python for educational purposes.

[PySOT](https://github.com/STVIR/pysot). SenseTime Research platform for single object tracking, implementing algorithms like SiamRPN and SiamMask.

[PyTracking](https://github.com/visionml/pytracking). A general python framework for training and running visual object trackers, based on PyTorch.

[PySlowFast](https://github.com/facebookresearch/SlowFast). PySlowFast: video understanding codebase from FAIR for reproducing state-of-the-art video models.

[PyMatting](https://github.com/pymatting/pymatting). PyMatting: A Python Library for Alpha Matting.

