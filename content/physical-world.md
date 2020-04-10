
# Inferring Physical World From Images

A collection of papers on inferring the physical world (shape, depth, motion, paint, light, colors, etc) from single RGB, multi-view or temporal images. 

## Table of Contents
- [Inverse Rendering](#inverse-rendering)
- [Disentanglement](#disentanglement)
- [Light, Reflectance, lluminance and Shade](#light--reflectance--lluminance-and-shade)
- [Shape and Viewpoint](#shape-and-viewpoint)
- [Human 3D Reconstruction](#human-3d-reconstruction)
  * [Soft-tissue Dynamics](#soft-tissue-dynamics)
  * [Human Dynamics](#human-dynamics)
  * [Human Poses and Shapes](#human-poses-and-shapes)
  * [Misc (Face, Object)](#misc--face--object-)
- [Hair Segmentation and Reconstruction](#hair-segmentation-and-reconstruction)
- [Human Pose Estimation](#human-pose-estimation)
- [3D Representations From Natural Images](#3d-representations-from-natural-images)
- [Depth](#depth)
  * [Depth From Video (Depth, Normal and Camera Motion Estimation)](#depth-from-video--depth--normal-and-camera-motion-estimation-)
  * [Depth with ToF](#depth-with-tof)
  * [Temporal- and Scale-Consistent Depth Estimation](#temporal--and-scale-consistent-depth-estimation)
  * [Depth and Related Tasks](#depth-and-related-tasks)
- [Learning Temporal Information from Videos](#learning-temporal-information-from-videos)
  * [FastSlow, Multiple Stream and Temporal Pyramid](#fastslow--multiple-stream-and-temporal-pyramid)
  * [3D convolutions (C3D)](#3d-convolutions--c3d-)
  * [Flow](#flow)
  * [2DCNN + LSTM (Temporal Block)](#2dcnn---lstm--temporal-block-)
- [Team and People](#team-and-people)
- [Good Start of 3D Resources (Python)](#good-start-of-3d-resources--python-)

## Inverse Rendering

**Learning to Predict 3D Objects with an Interpolation-based Differentiable Renderer.**<br>
*Wenzheng Chen, Jun Gao, Huan Ling, Edward J. Smith, Jaakko Lehtinen, Alec Jacobson, Sanja Fidler.*<br>
NeurIPS 2019. [[PDF](https://arxiv.org/abs/1908.01210)]

**InverseRenderNet: Learning Single Image Inverse Rendering.**<br>
*Ye Yu, William A. P. Smith.*<br>
CVPR 2019. [[PDF](http://openaccess.thecvf.com/content_CVPR_2019/html/Yu_InverseRenderNet_Learning_Single_Image_Inverse_Rendering_CVPR_2019_paper.html)] [[Github](https://github.com/YeeU/InverseRenderNet)] [[IIW Dataset](http://opensurfaces.cs.cornell.edu/publications/intrinsic/#download)] 

**Learning Inverse Rendering of Faces from Real-world Videos.**<br>
*Yuda Qiu, Zhangyang Xiong, Kai Han, Zhongyuan Wang, Zixiang Xiong, Xiaoguang Han.*<br>
arxiv, 2020. [[PDF](https://arxiv.org/abs/2003.12047)] [[Github](https://github.com/RudyQ/InverseFaceRender)]

## Hidden Surface Reasoning

**Where Does It End? -- Reasoning About Hidden Surfaces by Object Intersection Constraints.**<br>
*Michael Strecke, Joerg Stueckler.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.04630)]

## Scene Understanding

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

## Light, Reflectance, lluminance and Shade
**Lighthouse: Predicting Lighting Volumes for Spatially-Coherent Illumination.**<br>
*Pratul P. Srinivasan, Ben Mildenhall, Matthew Tancik, Jonathan T. Barron, Richard Tucker, Noah Snavely.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.08367)] [[Project](https://people.eecs.berkeley.edu/~pratul/lighthouse/)]

**Neural Illumination: Lighting Prediction for Indoor Environments.**<br>
*Shuran Song and Thomas Funkhouser.*<br>
CVPR 2019. [[PDF](https://illumination.cs.princeton.edu/paper.pdf)] [[Project](https://illumination.cs.princeton.edu/)]

**Learning to Shade Hand-drawn Sketches.**<br>
*Qingyuan Zheng, Zhuoru Li, Adam Bargteil.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2002.11812)]

**Generating Digital Painting Lighting Effects via RGB-space Geometry.**<br>
*Lvmin Zhang, Edgar Simo-Serra, Yi Ji, and Chunping Liu.*<br>
SIGGRAPH 2020 (TOG 2020).
[[Priject](https://lllyasviel.github.io/PaintingLight/)]
[[Github](https://github.com/lllyasviel/PaintingLight)]

**Illumination Decomposition for Photograph with Multiple Light Sources.**<br>
*Ling Zhang, Qingan Yan, Zheng Liu, Hua Zou, Chunxia Xiao.*<br>
TIP 2017. [[PDF](https://yanqingan.github.io/docs/tip17_illumination.pdf)] [[Github](https://github.com/yanqingan/Illumination_Decomposition)]

**Learning to Predict Indoor Illumination from a Single Image.**<br>
*Marc-André Gardner, [Kalyan Sunkavalli](https://research.adobe.com/person/kalyan-sunkavalli/), [Ersin Yumer](https://research.adobe.com/person/ersin-yumer/), [Xiaohui Shen](https://research.adobe.com/person/xiaohui-shen/), Emiliano Gambaretto, [Christian Gagné](http://vision.gel.ulaval.ca/~cgagne/), and [Jean-François Lalonde](http://vision.gel.ulaval.ca/~jflalonde/).*<br>
ACM Transactions on Graphics (SIGGRAPH Asia), 2017. [[PDF](https://arxiv.org/abs/1704.00090)] [[Dataset](http://indoor.hdrdb.com/)] [[Homepage](vision.gel.ulaval.ca/~jflalonde/projects/deepIndoorLight)]

**Deep Parametric Indoor Lighting Estimation.**<br>
*Marc-André Gardner, Yannick Hold-Geoffroy, Kalyan Sunkavalli, Christian Gagné, and Jean-François Lalonde.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1910.08812)] [[Supplementary material](https://lvsn.github.io/deepparametric/supplementary/index.html)] [[Laval Indoor HDR Database](http://indoor.hdrdb.com/) and [Depth](http://indoordepth.hdrdb.com/)] [[Project](https://lvsn.github.io/deepparametric/)] 

**Fast Spatially-Varying Indoor Lighting Estimation.**<br>
*Mathieu Garon, Kalyan Sunkavalli, Sunil Hadap, Nathan Carr, [Jean-François Lalonde](http://www.jflalonde.ca/).*<br>
CVPR 2019. [[PDF](https://arxiv.org/abs/1906.03799)] [[Supplementary material](https://lvsn.github.io/fastindoorlight/supplementary/index.html)] [[Project](https://lvsn.github.io/fastindoorlight/)] [[Lavel Indoor Spatially Varying HDR Dataset / 79 HDR Light Probes](http://indoorsv.hdrdb.com/)]

**GLoSH: Global-Local Spherical Harmonics for Intrinsic Image Decomposition.**<br>
*[Hao Zhou](http://zhhoper.github.io), Xiang Yu, David W Jacobs.*<br>
ICCV 2019. [[PDF](https://zhhoper.github.io/paper/zhou_ICCV2019_IID.pdf)] [[Supplement](https://zhhoper.github.io/paper/zhou_ICCV_2019_IID_sup.pdf)] [[Poster](https://zhhoper.github.io/poster/Poster_ICCV_2019_IID.pdf)] [[Spherical Harmonic Tools](shtools.github.io/SHTOOLS)]

**Deep Single-Image Portrait Relighting.**<br>
*Hao Zhou, Sunil Hadap, Kalyan Sunkavalli, David W. Jacobs.*<br>
ICCV 2019. [[PDF](https://arxiv.org/pdf/1905.00824)] [[Github](https://github.com/zhhoper/DPR)] [[Project](https://zhhoper.github.io/dpr.html)] [[DPR Dataset](https://drive.google.com/drive/folders/10luekF8vV5vo2GFYPRCe9Rm2Xy2DwHkT?usp=sharing)]

**Single Image Portrait Relighting.**<br>
*[Tiancheng Sun](http://kevinkingo.com/), Jonathan T. Barron, Yun-Ta Tsai, Zexiang Xu, Xueming Yu, Graham Fyffe, Christoph Rhemann, Jay Busch, Paul Debevec, [Ravi Ramamoorthi](https://cseweb.ucsd.edu/~ravir/).*<br> 
SIGGRAPH 2019. [[PDF](https://arxiv.org/abs/1905.00824)]

**Multi-view Relighting using a Geometry-Aware Network Paper Abstract Author Preprint Paper Video.**<br>
*Julien Philip, Michael Gharbi, Tinghui Zhou, Alexei (Alyosha) Efros, George Drettakis.*<br>

**SfSNet: Learning Shape, Reflectance and llluminance of Faces in the Wild.**<br>
*Soumyadip Sengupta, Angjoo Kanazawa, Carlos D. Castillo, David W. Jacobs.*<br>
CVPR 2018. [[Project](https://senguptaumd.github.io/SfSNet/)] [[PDF](https://arxiv.org/abs/1703.10131)] [[Github](https://github.com/matansel/pix2vertex)]

**Occlusion-aware 3D Morphable Models and an Illumination Prior for Face Image Analysis.**<br>
*Bernhard Egger, Sandro Schoenborn, Andreas Schneider, Adam Kortylewski, Andreas Morel-Forster, Clemens Blumer and Thomas Vetter.*<br>
IJCV 2018. [[BIP Dataset](https://gravis.dmi.unibas.ch/PMM/data/bip/)] [[PDF](http://gravis.dmi.unibas.ch/publications/2018/2018_Egger_IJCV.pdf)]

## Shape and Viewpoint
**Self-supervised 3D Shape and Viewpoint Estimation from Single Images for Robotics.**<br>
*Oier Mees, Maxim Tatarchenko, Thomas Brox and Wolfram Burgard.*<br>
IROS 2019. [[PDF](https://arxiv.org/abs/1910.07948.pdf)]

**Self-Supervised Viewpoint Learning From Image Collections.**<br>
*Siva Karthik Mustikovela, Varun Jampani, Shalini De Mello, Sifei Liu, Umar Iqbal, Carsten Rother, Jan Kautz.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.01793)]

## Human 3D Reconstruction

[[Awesome 3D Human Resources List](https://github.com/lijiaman/awesome-3d-human)]

### Soft-tissue Dynamics

**SoftSMPL: Data-driven Modeling of Nonlinear Soft-tissue Dynamics for Parametric Humans.**<br>
*[Igor Santesteban](http://isantesteban.com/), Elena Garces, Miguel A. Otaduy, and Dan Casas.*<br>
Computer Graphics Forum (Proc. of Eurographics), 2020. [[PDF](http://dancasas.github.io/docs/santesteban_Eurographics2020.pdf)] [[Project](http://dancasas.github.io/projects/SoftSMPL)]

### Human Dynamics 

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
CVPR 2019. [[PDF](https://arxiv.org/abs/1812.01601)] [[HomePage](https://akanazawa.github.io/human_dynamics/)]

**Predicting 3D Human Dynamics from Video.**<br>
*Jason Y. Zhang, Panna Felsen, Angjoo Kanazawa, Jitendra Malik.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1908.04781)] [[HomePage](https://jasonyzhang.com/phd/)]

**DeepHuman: 3D Human Reconstruction from a Single Image.**<br>
*[Zerong Zheng](https://zhengzerong.github.io/), [Tao Yu](https://ytrock.com/), Yixuan Wei, Qionghai Dai, [Yebin Liu](http://www.liuyebin.com/).*<br>
ICCV 2019. [[PDF](http://www.liuyebin.com/deephuman/assets/DeepHuman.pdf)] [[Project](http://www.liuyebin.com/deephuman/deephuman.html)] [[Code](https://github.com/ZhengZerong/DeepHuman)] [[THUmanDataset](https://github.com/ZhengZerong/DeepHuman/tree/master/THUmanDataset)] [[im2smpl](https://github.com/ZhengZerong/im2smpl)]

**LiveCap: Real-time Human Performance Capture from Monocular Video.**<br>
*Marc Habermann, Weipeng Xu, Michael and Zollhoefer, Gerard Pons-Moll, Christian Theobalt.*<br>
SIGGRAPH 2019. [[PDF](https://gvv.mpi-inf.mpg.de/projects/LiveCap/)] [[Project](https://gvv.mpi-inf.mpg.de/projects/LiveCap/)]

**Superpixel Soup: Monocular Dense 3D Reconstruction of a Complex Dynamic Scene.**<br>
*Suryansh Kumar, Yuchao Dai, Hongdong Li.*<br>
TPAMI 2019 (ICCV 2017). [[PDF](https://arxiv.org/abs/1911.09092)] 

### Human Poses and Shapes

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

### Misc (Face, Object)

**Learning Generative Models of Shape Handles.**<br>
*Matheus Gadelha, Giorgio Gori, Duygu Ceylan, Radomir Mech, Nathan Carr, Tamy Boubekeur, Rui Wang, Subhransu Maji.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.03028)]

**A Morphable Face Albedo Model.**<br>
*William A.P. Smith, Alassane Seck, Hannah Dee, Bernard Tiddeman, Joshua Tenenbaum, Bernhard Egger.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.02711)]

**HandVoxNet: Deep Voxel-Based Network for 3D Hand Shape and Pose Estimation from a Single Depth Map.**<br>
*Jameel Malik, Ibrahim Abdelaziz, Ahmed Elhayek, Soshi Shimada, Sk Aziz Ali, Vladislav Golyanik, Christian Theobalt, Didier Stricker.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.01588)]

**AvatarMe: Realistically Renderable 3D Facial Reconstruction "in-the-wild".**<br>
*Alexandros Lattas, Stylianos Moschoglou, Baris Gecer, Stylianos Ploumpis, Vasileios Triantafyllou, Abhijeet Ghosh, Stefanos Zafeiriou.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.13845)] [[Github](http://github.com/lattas/AvatarMe)]

**DOPS: Learning to Detect 3D Objects and Predict their 3D Shapes.**<br>
*Mahyar Najibi, Guangda Lai, Abhijit Kundu, Zhichao Lu, Vivek Rathod, Tom Funkhouser, Caroline Pantofaru, David Ross, Larry S. Davis, Alireza Fathi.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.01170)]

**Modeling 3D Shapes by Reinforcement Learning.**<br>
*Cheng Lin, Tingxiang Fan, Wenping Wang, Matthias Nießner.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2003.12397)]

**FacePSNet: Lightweight Photometric Stereo for Facial Details Recovery.**<br>
*Xueying Wang, Yudong Guo, Bailin Deng, Juyong Zhang.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.12307)] [[Github](https://github.com/Juyong/FacePSNet)]

**High Accuracy Face Geometry Capture using a Smartphone Video.**<br>
*Shubham Agrawal, Anuj Pahuja, Simon Lucey.*<br>
WACV 2020. [[PDF](https://arxiv.org/abs/2003.08583)]

**Unsupervised Learning of Probably Symmetric Deformable 3D Objects from Images in the Wild.**<br>
*[Shangzhe Wu](https://elliottwu.com/), Christian Rupprecht, Andrea Vedaldi.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/1911.11130)] [[Project](https://elliottwu.com/projects/unsup3d/)]

**Rotate-and-Render: Unsupervised Photorealistic Face Rotation from Single-View Images.**<br>
*Hang Zhou, Jihao Liu, Ziwei Liu, Yu Liu, Xiaogang Wang.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.08124)] [[Github](https://github.com/Hangz-nju-cuhk/Rotate-and-Render)]
**Self-supervised Single-view 3D Reconstruction via Semantic Consistency.**<br>
*Xueting Li, Sifei Liu, Kihwan Kim, Shalini De Mello, Varun Jampani, Ming-Hsuan Yang, Jan Kautz.*<br>
arxiv, 13 Mar 2020. [[PDF](https://arxiv.org/abs/2003.06473)] [[Project](https://sites.google.com/view/unsup-mesh/home)]

**Towards High-Fidelity 3D Face Reconstruction from In-the-Wild Images Using Graph Convolutional Networks.**<br>
*Jiangke Lin, Yi Yuan, Tianjia Shao, Kun Zhou.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.05653)]

**Inverse Graphics GAN: Learning to Generate 3D Shapes from Unstructured 2D Data.**<br>
*Sebastian Lunz, Yingzhen Li, Andrew Fitzgibbon, Nate Kushman.*<br>
arxiv, 28 Feb 2020. [[PDF](https://arxiv.org/abs/2002.12674)]

**Multi-layer Depth and Epipolar Feature Transformers for 3D Scene Reconstruction.**<br>
*Daeyun Shin, Zhile Ren, Erik B. Sudderth, Charless C. Fowlkes.*<br>
CVPR 2019. [[PDF](http://openaccess.thecvf.com/content_CVPRW_2019/papers/SUMO/Shin_Multi-layer_Depth_and_Epipolar_Feature_Transformers_for_3D_Scene_Reconstruction_CVPRW_2019_paper.pdf)]

**SDFDiff: Differentiable Rendering of Signed Distance Fields for 3D Shape Optimization.**<br>
*Yue Jiang, Dantong Ji, Zhizhong Han, Matthias Zwicker.*<br>
arxiv, 15 Dec 2019. [[PDF](https://arxiv.org/abs/1912.07109)]

**Learning to Reconstruct 3D Manhattan Wireframes from a Single Image.**<br>
*Yichao Zhou, [Haozhi Qi](https://people.eecs.berkeley.edu/~hqi/), Yuexiang Zhai, Qi Sun, Zhili Chen, [Li-Yi Wei](https://research.adobe.com/person/li-yi-wei/), [Yi Ma](https://people.eecs.berkeley.edu/~yima/).*<br>
ICCV 2019. [[PDF](https://people.eecs.berkeley.edu/~hqi/)] [[Video Demonstration](https://youtu.be/l3sUtddPJPY)]

**Semi-Supervised Monocular 3D Face Reconstruction With End-to-End Shape-Preserved Domain Transfer.**<br>
*Jingtan Piao, Chen Qian, Hongsheng Li.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Piao_Semi-Supervised_Monocular_3D_Face_Reconstruction_With_End-to-End_Shape-Preserved_Domain_Transfer_ICCV_2019_paper.pdf)]

**Learning Joint Reconstruction of Hands and Manipulated Objects.**<br>
*Yana Hasson, Gül Varol, Dimitris Tzionas, Igor Kalevatykh, Michael J. Black, Ivan Laptev, Cordelia Schmid.*<br>
CVPR 2019. [[PDF](https://arxiv.org/abs/1904.05767)] [[Project](https://hassony2.github.io/obman.html)] [[ObMan dataset](https://github.com/hassony2/obman)] [[Github](https://github.com/hassony2/obman_train)]

**Facial Details Synthesis From Single Input Image.**<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1903.10873)] [[Supplemental Material](https://github.com/apchenstu/Facial_Details_Synthesis/blob/master/src/imgs/Supplemental_Material.pdf)] [[Github](https://github.com/apchenstu/Facial_Details_Synthesis)]

**Photo-Realistic Facial Details Synthesis from Single Image.**<br>
*Anpei Chen, Zhang Chen, Guli Zhang, Ziheng Zhang, Kenny Mitchell, Jingyi Yu.*<br> 
ICCV 2019. [[PDF](https://arxiv.org/abs/1903.10873)] [[Supplemental Material](https://github.com/apchenstu/Facial_Details_Synthesis/blob/master/src/imgs/Supplemental_Material.pdf)] [[Github](https://github.com/apchenstu/Facial_Details_Synthesis)]

**FML: Face Model Learning From Video.**<br>
*A. Tewari, F. Bernard, P. Garrido, G. Bharaj, M. Elgharib, H-P. Seidel, P. Perez, M. Zollhöfer, C.Theobalt.*  <br>
CVPR 2019. [[PDF](http://gvv.mpi-inf.mpg.de/projects/FML19/paper.pdf)] [[MPI Informatics, Saarland Informatics Campus](http://www.mpi-inf.mpg.de/home/)] [[Project](gvv.mpi-inf.mpg.de/projects/FML19)] 

**Unsupervised 3D Reconstruction Networks.**<br>
*Geonho Cha, Minsik Lee, Songhwai Oh.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Cha_Unsupervised_3D_Reconstruction_Networks_ICCV_2019_paper.pdf)]

**Domain-Adaptive Single-View 3D Reconstruction.**<br>
*Pedro O. Pinheiro, Negar Rostamzadeh, Sungjin Ahn.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Pinheiro_Domain-Adaptive_Single-View_3D_Reconstruction_ICCV_2019_paper.pdf)]

**Neural 3D Mesh Renderer.**<br>
*Hiroharu Kato, Yoshitaka Ushiku, Tatsuya Harada.*<br>
CVPR 2018. [[PDF](https://arxiv.org/abs/1711.07566)] [[Project](http://hiroharu-kato.com/projects_en/neural_renderer.html)] [[Github](https://github.com/hiroharu-kato/neural_renderer)]

## Hair Segmentation and Reconstruction

**Dynamic Hair Modeling from Monocular Videos using Deep Neural Networks.**<br>
*Lingchen Yang, Zefeng Shi, [Youyi Zheng](http://youyizheng.net/research.html), [Kun Zhou](http://kunzhou.net/).*<br>
ACM Transactions on Graphics (SIGGRAPH ASIA 2019). [[PDF](http://www.cad.zju.edu.cn/home/zyy/docs/dynamic_hair.pdf)]

**Hair-GAN: Recovering 3D Hair Structure from a Single Image using Generative Adversarial Networks.**<br>
*Meng Zhang, Youyi Zheng.*<br>
Visual Informatics 2019. [[PDF](http://www.cad.zju.edu.cn/home/zyy/docs/hairgan_final.pdf)]

**Semantic Soft Segmentation.**<br>
*Yagiz Aksoy, Tae-Hyun Oh, Sylvain Paris, Marc Pollefeys and Wojciech Matusik.*<br>
ACM Transactions on Graphics (Proc. SIGGRAPH), 2018. [[PDF](http://yaksoy.github.io/papers/TOG18-sss-supp.pdf)] [[Project](http://yaksoy.github.io/sss/)] [[Github](https://github.com/yaksoy/SemanticSoftSegmentation)] 

**Learning-based Sampling for Natural Image Matting.**<br>
*Jingwei Tang, Yagiz Aksoy, Cengiz Oztireli, Markus Gross, and Tunc Ozan Aydin.*<br>
CVPR, 2019. [[PDF](http://yaksoy.github.io/papers/CVPR19-samplenet.pdf)] [[Project](http://yaksoy.github.io/samplenet/)] 

**Soft Segmentation of Images.**<br>
*Yagiz Aksoy.*<br>
PhD Thesis, ETH Zurich, 2019. [[PDF](http://yaksoy.github.io/papers/ETH19-PhD-Aksoy.pdf)] [[Project](yaksoy.github.io/ssi/)]

**3D Hair Synthesis Using Volumetric Variational Autoencoders.**<br>
*Shunsuke Saito, Liwen Hu, Chongyang Ma, Hikaru Ibayashi, Linjie Luo, Hao Li.*<br>
ACM Transaction on Graphics (SIGGRAPH Asia 2018). [[PDF](http://www.hao-li.com/publications/papers/siggraphAsia2018PAGAN.pdf)]

**HairNet: Single-View Hair Reconstruction using Convolutional Neural Networks.**<br>
*Yi Zhou, Liwen Hu, Jun Xing, Weikai Chen, Han-Wei Kung, Xin Tong, Hao Li.*<br>
2018. [[PDF](https://arxiv.org/abs/1806.07467)] [[GitHub](http://t.cn/AiBvbwNK)] 

## Human Pose Estimation

[[Awesome work on hand pose estimation/tracking.](https://github.com/xinghaochen/awesome-hand-pose-estimation)]

**Camera-to-Robot Pose Estimation from a Single Image.**<br>
*Timothy E. Lee, Jonathan Tremblay, Thang To, Jia Cheng, Terry Mosier, Oliver Kroemer, Dieter Fox, Stan Birchfield.*<br>
[[PDF](https://arxiv.org/abs/1911.09231)]

**Mask-pose Cascaded CNN for 2D Hand Pose Estimation from Single Color Images.**<br>
**Yangang Wang, Cong Peng, Yebin Liu.**<br>
IEEE Trans. CSVT 2019. [[Project](https://www.yangangwang.com/papers/WANG-MCC-2018-10.html)]
[[PDF](http://www.liuyebin.com/hand2d/hand2d.pdf)] 

## 3D Representations From Natural Images

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

## Depth

### Depth From Video (Depth, Normal and Camera Motion Estimation)

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

**Surface Normals and Shape From Water.**<br>
*Satoshi Murai, Meng-Yu Jennifer Kuo, Ryo Kawahara, Shohei Nobuhara, Ko Nishino.*<br> 
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Murai_Surface_Normals_and_Shape_From_Water_ICCV_2019_paper.pdf)]

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

**Surface Normals in the Wild.**<br>
*Weifeng Chen, Donglai Xiang, Jia Deng.*<br>
ICCV 2017, Invited Poster at the Bridges to 3D Workshop, CVPR 2018.
[[PDF](https://arxiv.org/abs/1704.02956)] [[Dataset](http://www-personal.umich.edu/~wfchen/surface-normals-in-the-wild/)] [[Gihtub](https://github.com/princeton-vl/surface_normals)]

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

