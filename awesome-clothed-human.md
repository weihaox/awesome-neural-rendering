
# awesome clothed people papers [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A collection of resources on clothed people. 

## Contributing

If you think I have missed out on something (or) have any suggestions (papers, implementations and other resources), feel free to [pull a request](https://github.com/xiaweihao/awesome-image-translation/pulls)

Feedback and contributions are welcome!

## Table of Contents
- [3D People Dressing and Clothing Draping](#3d-people-dressing-and-clothing-draping)
- [Clothed People Digitalization](#clothed-people-digitalization)
- [Fashion Style Influences](#fashion-style-influences)
- [Image-Based Virtual Try-On](#image-based-virtual-try-on)
  * [Challenge and workshop](#challenge-and-workshop)
  * [Datasets](#datasets)
- [Team and People](#team-and-people)
- [Dataset](#dataset)

## 3D People Dressing and Clothing Draping

**Neural Non-Rigid Tracking.**<br>
*Aljaž Božič, Pablo Palafox, Michael Zollhöfer, Angela Dai, Justus Thies, Matthias Nießner.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2006.13240)]

**Homogenized Yarn-Level Cloth.**<br>
*[Georg Sperl](https://pub.ist.ac.at/~gsperl/), Rahul Narain, Chris Wojtan.*<br>
ACM Transactions on Graphics (SIGGRAPH 2020). [[PDF](http://pub.ist.ac.at/group_wojtan/projects/2020_Sperl_HYLC/2020_HYLC_paper.pdf)] [[Project](http://visualcomputing.ist.ac.at/publications/2020/HYLC/)] [[Data & Code](http://pub.ist.ac.at/group_wojtan/projects/2020_Sperl_HYLC/2020_HYLC_data_code.zip)]

**DeepDeform: Learning Non-rigid RGB-D Reconstruction with Semi-supervised Data.**<br>
*Aljaž Božič, Michael Zollhöfer, Christian Theobalt, Matthias Nießner.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/1912.04302)] [[Project](https://pure.mpg.de/pubman/faces/ViewItemOverviewPage.jsp?itemId=item_3187203)] [[Github](https://github.com/AljazBozic/DeepDeform)] [[DeepDeform Benchmark](http://kaldir.vc.in.tum.de/deepdeform_benchmark)]

**Deep Fashion3D: A Dataset and Benchmark for 3D Garment Reconstruction from Single Images.**<br>
*Heming Zhu, Yu Cao, Hang Jin, Weikai Chen, Dong Du, Zhangye Wang, Shuguang Cui, Xiaoguang Han.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2003.12753)] [[Project](https://kv2000.github.io/2020/03/25/deepFashion3DRevisited/)]

**Implicit Functions in Feature Space for 3D Shape Reconstruction and Completion.**<br>
*Julian Chibane, [Thiemo Alldieck](https://graphics.tu-bs.de/people/alldieck), Gerard Pons-Moll.*<br>
CVPR 2020. [[PDF](https://virtualhumans.mpi-inf.mpg.de/papers/chibane20ifnet/chibane20ifnet.pdf)]

**Learning to Dress 3D People in Generative Clothing.**<br>
*Qianli Ma, Jinlong Yang, Anurag Ranjan, Sergi Pujades, Gerard Pons-Moll, Siyu Tang, Michael J. Black.*<br>
CVPE 2020. [[PDF](https://arxiv.org/abs/1907.13615)]

**DeepCap: Monocular Human Performance Capture Using Weak Supervision.**<br>
*Marc Habermann, Weipeng Xu, Michael and Zollhoefer, Gerard Pons-Moll, Christian Theobalt.*<br>
CVPR 2020. [[PDF](https://virtualhumans.mpi-inf.mpg.de/)]

**The Virtual Tailor: Predicting Clothing in 3D as a Function of Human Pose, Shape and Garment Style.**<br>
*Chaitanya Patel, Zhouyingcheng Liao, Gerard Pons-Moll.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.04583)]

**Learning to Transfer Texture from Clothing Images to 3D Humans.**<br>
*Aymen Mir, Thiemo Alldieck, Gerard Pons-Moll.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.02050)] [[Github](https://github.com/aymenmir1/pix2surf)]

**GarNet: A Two-Stream Network for Fast and Accurate 3D Cloth Draping.**<br>
*[Erhan Gundogdu](https://egundogdu.github.io/), Victor Constantin, Amrollah Seifoddini, Minh Dang, Mathieu Salzmann, Pascal Fua.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1811.10983)] [[Supplementary Material](https://www.epfl.ch/labs/cvlab/wp-content/uploads/2019/04/GarNet_supplementary.pdf)] [[Project](https://cvlab.epfl.ch/research/garment-simulation/garnet/)] [[Dataset](https://drive.switch.ch/index.php/s/7mAk9SoZ7J4uokt)]

**Multi-Garment Net: Learning to Dress 3D People from Images.**<br>
*Bharat Lal Bhatnagar, Garvita Tiwari, Christian Theobalt, [Gerard Pons-Moll](https://www.mpi-inf.mpg.de/departments/computer-vision-and-machine-learning/people/gerard-pons-moll/)(REAL VIRTUAL HUMANS, MPII).*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1908.06903)]

**CAPE: Learning to Dress 3D People in Generative Clothing.**<br>
*[Qianli Ma](https://ps.is.tue.mpg.de/person/qma), Jinlong Yang, Anurag Ranjan, Sergi Pujades, Gerard Pons-Moll, Siyu Tang, [Michael J. Black](https://ps.is.tuebingen.mpg.de/person/black).*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/1907.13615v2)] 	[[Projecr](http://ps.is.mpg.de/publications/cape-cvpr-20)]

**DRAPE: DRessing Any PErson.**<br>
*Peng Guan, Loretta Reiss, David A. Hirshberg, Alexander Weiss, Michael J. Black.*<br>
ACM Transactions on Graphics (TOG) 2012.
[[PDF](https://dl.acm.org/citation.cfm?doid=2185520.2185531)]
[[Project](https://ps.is.tue.mpg.de/research_projects/drape-dressing-any-person)]

**CLOTH3D: Clothed 3D Humans.**<br>
*Hugo Bertiche, Meysam Madadi, Sergio Escalera.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/1912.02792v1)]

## Clothed People Digitalization

**TailorNet: Predicting Clothing in 3D as a Function of Human Pose, Shape and Garment Style.**<br>
*Chaitanya Patel*, Zhouyingcheng Liao*, Gerard Pons-Moll.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.04583)] [[Github](https://github.com/chaitanya100100/TailorNet)] [[Project](https://virtualhumans.mpi-inf.mpg.de/tailornet/)] [[Data](https://github.com/zycliao/TailorNet_dataset)]

**Geo-PIFu: Geometry and Pixel Aligned Implicit Functions for Single-view Human Reconstruction.**<br>
*Tong He, John Collomosse, Hailin Jin, Stefano Soatto.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2006.08072)]

**SparseFusion: Dynamic Human Avatar Modeling from Sparse RGBD Images.**<br>
*Xinxin Zuo, Sen Wang, Jiangbin Zheng, Weiwei Yu, Minglun Gong, Ruigang Yang, Li Cheng.*<br>
TMM 2020. [[PDF](https://arxiv.org/abs/2006.03630)]

**Self-Supervised Human Depth Estimation from Monocular Videos.**<br>
*Feitong Tan, Hao Zhu, Zhaopeng Cui, Siyu Zhu, Marc Pollefeys, Ping Tan.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2005.03358)]

**TetraTSDF: 3D human reconstruction from a single image with a tetrahedral outer shell.**<br>
*Hayato Onizuka, Zehra Hayirci, Diego Thomas, Akihiro Sugimoto, Hideaki Uchiyama, Rin-ichiro Taniguchi.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2004.10534)]

**ARCH: Animatable Reconstruction of Clothed Humans.**<br>
*Zeng Huang, Yuanlu Xu, Christoph Lassner, Hao Li, Tony Tung.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.04572)]

**PIFuHD: Multi-Level Pixel-Aligned Implicit Function for High-Resolution 3D Human Digitization.**<br>
*Shunsuke Saito, Tomas Simon, Jason Saragih, Hanbyul Joo.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.00452)] [[Project](https://shunsukesaito.github.io/PIFuHD)] [[Github](https://github.com/shunsukesaito/PIFuHD)]

**DeepCap: Monocular Human Performance Capture Using Weak Supervision.**<br>
*Marc Habermann, Weipeng Xu, Michael Zollhoefer, erard Pons-Moll, Christian Theobalt.*<br>
CVPR 2020. [[PDF](https://gvv.mpi-inf.mpg.de/projects/2020-cvpr-deepcap/data/paper.pdf)] [[PDF](https://gvv.mpi-inf.mpg.de/projects/2020-cvpr-deepcap/)]

**EventCap: Monocular 3D Capture of High-Speed Human Motions using an Event Camera.**<br>
*Lan XU, Weipeng Xu, Vladislav Golyanik, Marc Habermann, Lu Fang, Christian Theobalt.*<br>
CVPR 2020. [[PDF](https://gvv.mpi-inf.mpg.de/projects/2020-cvpr-eventcap/data/paper.pdf)] [[PDF](https://gvv.mpi-inf.mpg.de/projects/2020-cvpr-eventcap/)]

**Learning to Transfer Texture from Clothing Images to 3D Humans.**<br>
*Aymen Mir, Thiemo Alldieck, Gerard Pons-Moll.*<br>
arxiv, 4 Mar 2020. [[PDF](https://arxiv.org/abs/2003.02050)]

**PeelNet: Textured 3D reconstruction of human body using single view RGB image.**<br>
*Sai Sagar Jinka, Rohan Chacko, Avinash Sharma, P. J. Narayanan.*<br>
arxiv, 16 Feb 2020. [[PDF](https://arxiv.org/abs/2002.06664)]

**BCNet: Learning Body and Cloth Shape from A Single Image.**<br>
*Boyi Jiang, Juyong Zhang, Yang Hong, Jinhao Luo, Ligang Liu, Hujun Bao.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2004.00214)]

**Disentangled Human Body Embedding Based on Deep Hierarchical Neural Network.**<br>
*Boyi Jiang, Juyong Zhang, Jianfei Cai, Jianmin Zheng.*<br>
TVCG 2020. [[PDF](https://arxiv.org/abs/1905.05622)]

**Textured Neural Avatars.**<br>
*Aliaksandra Shysheya, Egor Zakharov, Kara-Ali Aliev, Renat Bashirov, Egor Burkov, Karim Iskakov, Aleksei Ivakhnenko, Yury Malkov, Igor Pasechnik, Dmitry Ulyanov, Alexander Vakhitov, Victor Lempitsky.*<br>
CVPR 2019 (oral). [[PDF](https://arxiv.org/abs/1905.08776)] [[Project](https://saic-violet.github.io/texturedavatar/)]

**PIFu: Pixel-Aligned Implicit Function for High-Resolution Clothed Human Digitization.**<br>
*Shunsuke Saito, Zeng Huang, Ryota Natsume, Shigeo Morishima, Angjoo Kanazawa, Hao Li.*<br>
ICCV 2019. [[PDF](https://arxiv.org/pdf/1905.05172.pdf)] [[Project](shunsukesaito.github.io/PIFu)] [[Github](https://github.com/shunsukesaito/PIFu)]

**SimulCap : Single-View Human Performance Capture with Cloth Simulation.** <br>
*Tao Yu, Zerong Zheng, Yuan Zhong, Jianhui Zhao, Qionghai Dai, Gerard Pons-moll, Yebin Liu.*<br>
CVPR 2019. [[PDF](http://www.liuyebin.com/simulcap/assets/SimulCap.pdf)] [[Project](http://www.liuyebin.com/simulcap/simulcap.html)]

**SiCloPe: Silhouette-Based Clothed People.** <br>
*Ryota Natsume, [Shunsuke Saito](http://www-scf.usc.edu/~saitos/), Zeng Huang, Weikai Chen, Chongyang Ma, Hao Li, Shigeo Morishima.* <br>
CVPR 2019. [[PDF](http://openaccess.thecvf.com/content_CVPR_2019/papers/Natsume_SiCloPe_Silhouette-Based_Clothed_People_CVPR_2019_paper.pdf)]

**Multi-Garment Net_Learning to Dress 3D people from Images.**<br>
*Bharat Lal Bhatnagar, Garvita Tiwari, Christian Theobalt, Gerard Pons-Moll.*<br>
ICCV 2019. 
[[Github](https://github.com/bharat-b7/MultiGarmentNetwork)] [[PDF](https://virtualhumans.mpi-inf.mpg.de/papers/bhatnagar2019mgn/bhatnagar2019mgn.pdf)]

**3DPeople: Modeling the Geometry of Dressed Humans.** <br>
*Albert Pumarola, Jordi Sanchez, Gary P. T. Choi, Alberto Sanfeliu, Francesc Moreno-Noguer.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1904.04571)] [[3DPeople-Dataset](https://github.com/albertpumarola/3DPeople-Dataset)]

**Tex2Shape: Detailed Full Human Body Geometry From a Single Image.** <br>
*Thiemo Alldieck, Gerard Pons-Moll, Christian Theobalt, Marcus Magnor.* <br>
CVPR 2019. [[PDF](https://arxiv.org/abs/1904.08645)] [[Github](https://github.com/thmoa/tex2shape)]

**Learning to Reconstruct People in Clothing from a Single RGB Camera.**<br>
*Thiemo Alldieck, Marcus Magnor, Bharat Lal Bhatnagar, Christian Theobalt, Gerard Pons-Moll.* <br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1903.05885)] [[Github](https://github.com/thmoa/octopus)]

**360-Degree Textures of People in Clothing from a Single Image.** <br>
*Verica Lazova, Eldar Insafutdinov, Gerard Pons-Moll.* <br>
3DV 2019. [[PDF](https://arxiv.org/pdf/1908.07117.pdf)] [[Project](http://virtualhumans.mpi-inf.mpg.de/360tex/)] 

**TexturePose: Supervising Human Mesh Estimation with Texture Consistency.** <br>
[[PDF](https://arxiv.org/abs/1910.11322) Georgios Pavlakos, Nikos Kolotouros, Kostas Daniilidis. <br>
[Project](https://www.seas.upenn.edu/~pavlakos/projects/texturepose/)

**Detailed Human Avatars from Monocular Video.**  <br>
*Thiemo Alldieck, Marcus Magnor, Weipeng Xu, Christian Theobalt, Gerard Pons-Moll.* <br>
3DV 2018. [[PDF](https://arxiv.org/abs/1808.01338)] [[Github](https://github.com/thmoa/semantic_human_texture_stitching)]

**A Neural Network for Detailed Human Depth Estimation From a Single Image.**<br>
*Sicong Tang, Feitong Tan, Kelvin Cheng, Zhaoyang Li, Siyu Zhu, Ping Tan.* <br>
ICCV 2109. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Tang_A_Neural_Network_for_Detailed_Human_Depth_Estimation_From_a_ICCV_2019_paper.pdf)]

**3D Reconstruction from a single image.** <br>
Oppo shared on ISMAR 2019.

## Fashion Style Influences

**From Paris to Berlin: Discovering Fashion Style Influences Around the World.**<br>
*Ziad Al-Halah, Kristen Grauman.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.01316)]

## Image-Based Virtual Try-On

**Learning Color Compatibility in Fashion Outfits.**<br>
*Heming Zhang, Xuewen Yang, Jianchao Tan, Chi-Hao Wu, Jue Wang, C.-C. Jay Kuo.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2007.02388)]

**Do Not Mask What You Do Not Need to Mask: a Parser-Free Virtual Try-On.**<br>
*Thibaut Issenhuth, Jérémie Mary, Clément Calauzènes.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.02721)]

**Toward Characteristic-Preserving Image-based Virtual Try-On Network.**<br>
*Bochao Wang, Huabin Zheng, Xiaodan Liang, Yimin Chen, Liang Lin, Meng Yang.*<br>
ECCV 2018. [[PDF](https://arxiv.org/abs/1807.07688)]

**Imitation Learning for Fashion Style Based on Hierarchical Multimodal Representation.**<br>
*Shizhu Liu, Shanglin Yang, Hui Zhou.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2004.06229)]

**LGVTON: A Landmark Guided Approach to Virtual Try-On.**<br>
*Debapriya Roy, Sanchayan Santra, Bhabatosh Chanda.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2004.00562)]

**Toward Accurate and Realistic Virtual Try-on Through Shape Matching and Multiple Warps.**<br>
*Kedan Li, Min Jin Chong, Jingen Liu, David Forsyth.*<br>
arxiv, 22 Mar 2020. [[PDF](https://arxiv.org/abs/2003.10817)]

**Towards Photo-Realistic Virtual Try-On by Adaptively Generating Preserving Image Content.**<br>
*Han Yang, Ruimao Zhang, Xiaobao Guo, Wei Liu, Wangmeng Zuo, Ping Luo.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.05863)] [[Github](https://github.com/switchablenorms/DeepFashion_Try_On)]

**PSGAN: Pose and Expression Robust Spatial-Aware GAN for Customizable Makeup Transfer.**<br>
*Wentao Jiang, Si Liu, Chen Gao, Jie Cao, Ran He, Jiashi Feng, Shuicheng Yan.*<br>
CVPR2020. [[PDF](https://arxiv.org/abs/1909.06956)]

**GarmentGAN: Photo-realistic Adversarial Fashion Transfer.**<br>
*Amir Hossein Raffiee, Michael Sollami.*<br>
arxiv, 4 Mar 2020. [[PDF](https://arxiv.org/abs/2003.01894)]

**TailorGAN: Making User-Defined Fashion Designs.**<br>
*Lele Chen, Justin Tian, Guo Li, Cheng-Haw Wu, Erh-Kan King, Kuan-Ting Chen, Shao-Hang Hsieh.*<br>
arxiv, 17 Jan 2019. [[PDF](https://arxiv.org/abs/2001.06427)]

**SieveNet: A Unified Framework for Robust Image-Based Virtual Try-On.**<br>
*Surgan Jandial, Ayush Chopra, Kumar Ayush, Mayur Hemani, Abhijeet Kumar, Balaji Krishnamurthy.*<br>
arxiv, 17 Jan 2019. [[PDF](https://arxiv.org/abs/2001.06265)]

**Generating High-Resolution Fashion Model Images Wearing Custom Outfits.**<br> 
*Gökhan Yildirim, Nikolay Jetchev, Roland Vollgraf, Urs Bergmann.*<br> 
Workshop on Computer Vision for Fashion, Art and Design, ICCV 2019. [[PDF](https://arxiv.org/abs/1908.09638)] 

### Challenge and workshop
- KDD Workshop on Fashion. [[2019]](https://kddfashion2019.mybluemix.net/) [[2018]](https://kddfashion2018.mybluemix.net/) [[2017]](https://kddfashion2017.mybluemix.net/) [[2016]](http://kddfashion2016.mybluemix.net/)
- Workshop on Computer Vision for Fashion, Art and Design. [[CVPR 2020]](https://sites.google.com/view/cvcreative2020) [[ICCV 2019]](https://sites.google.com/view/cvcreative/home) [[ECCV 2018]](https://sites.google.com/view/eccvfashion/) [[ICCV 2017]](https://sites.google.com/zalando.de/cvf-iccv2017/home?authuser=0)
- NeurlPS workshop on Machine Learning for Creativity and Design. [[2019]](https://neurips2019creativity.github.io/) [[2018]](https://nips2018creativity.github.io/) [[2017]](https://nips2017creativity.github.io/)
- SIGIR Workshop On eCommerce. [[2019]](https://sigir-ecom.github.io/index.html) [[2018]](https://sigir-ecom.github.io/ecom2018/index.html) [[2017]](http://sigir-ecom.weebly.com/) 
- CVPR Deep Learning for Content Creation Tutorial. [[2019]](https://nvlabs.github.io/dl-for-content-creation/)
- iMaterialist Fashion Challenge. [[CVPR 2019]](https://sites.google.com/view/fgvc6/competitions/imat-fashion-2019)
- iDesigner Challenge. [[CVPR 2019]](https://sites.google.com/view/fgvc6/competitions/idesigner-2019)
- FashionGen Challenge. [[ICCV 2019, ECCV 2018]](https://fashion-gen.com/)
- JD AI Fashion Challenge. [[ChinaMM 2018]](https://fashion-challenge.github.io/)
- Alibaba FashionAI Global Challenge. [[Tianchi]](http://fashionai.alibaba.com/)
- Artificial Intelligence on Fashion and Textile Conference. [[AIFT 2018]](https://www.polyu.edu.hk/itc/aift2018/)
- Fashion IQ Challenge. [[CVPR 2020]](https://sites.google.com/view/cvcreative2020/fashion-iq?authuser=0) [[ICCV 2019]](https://sites.google.com/view/lingir/fashion-iq)
- DeepFashion2 Challenge. [[CVPR 2020]](https://sites.google.com/view/cvcreative2020/deepfashion2?authuser=0) [[ICCV 2019]](https://sites.google.com/view/cvcreative/deepfashion2)

### Datasets
- Fashionpedia. [[Website]](https://fashionpedia.github.io/home/index.html)
- DeepFashion2 Dataset. [[Website]](<https://github.com/switchablenorms/DeepFashion2>)
- DeepFashion Dataset. [[Website]](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html)
- FashionGen. [[Website]](https://fashion-gen.com/)
- FashionAI. [[Tianchi]](http://fashionai.alibaba.com/datasets/?spm=a2c22.11190735.991137.8.501b6d83ilPJsX)
- TaobaoClothMatch. [[Tianchi]](TaobaoClothMatch)
- Fashion-MNIST. [[Fashion-MNIST]](https://github.com/zalandoresearch/fashion-mnist)
- Fashion IQ. [[Website]](https://www.spacewu.com/posts/fashion-iq/)

## Team and People 

- [Real Virtual Humans](http://virtualhumans.mpi-inf.mpg.de/), **Max Planck Institute for Informatics**, by [Gerard Pons-Moll](http://virtualhumans.mpi-inf.mpg.de/people/pons-moll.html).
- [Perceiving Systems, Tubingen Compus](http://ps.is.tuebingen.mpg.de/), **Max Planck Institute for Intelligent Systems**.
- [Visual Computer Lab](https://niessnerlab.org/opening.html), **Technical University Munich (TUM)**, by [Prof. Dr. Matthias Nießner](https://niessnerlab.org/members/matthias_niessner/profile.html) and his [team](https://niessnerlab.org/team.html).
- [Broadband Network and Digital Media Lab](http://www.liuyebin.com/student.html), Department of Automation, **Tsinghua University**, by [Yebin Liu](http://www.liuyebin.com/).
- [Vision and Graphics Lab](https://ict.usc.edu/), **University of Southern California**, by [Hao Li](http://hao-li.com/Hao_Li/Hao_Li_-_publications.html).

## Dataset

- **SMPL**. To download the [SMPL-X](https://smpl-x.is.tue.mpg.de/), [SMPL+H](http://mano.is.tue.mpg.de/) and SMPL ([Male and Female](http://smpl.is.tue.mpg.de/), [Gender Neural Model](http://smplify.is.tue.mpg.de/)) model, go to this project website and register to get access to the downloads section. [[Github](https://github.com/vchoutas/smplx#loading-smpl-x-smplh-and-smpl)]

- **THUmanDataset**. [THUman](https://github.com/ZhengZerong/DeepHuman/tree/master/THUmanDataset) is a 3D real-world human model dataset containing approximately 7000 models.

