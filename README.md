# awesome neural rendering papers [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A collection of resources on neural rendering. 

## Contributing

If you think I have missed out on something (or) have any suggestions (papers, implementations and other resources), feel free to [pull a request](https://github.com/xiaweihao/awesome-image-translation/pulls)

Feedback and contributions are welcome!

## Table of Contents
- [Related Surveys and Course Notes](#related-surveys-and-course-notes)
- [Inverse Rendering](#inverse-rendering)
- [Neural Rerendering](#neural-rerendering)
- [Fluid and Smoke Simulation](#fluid-and-smoke-simulation)
- [Differentiable Physics-Based Simulation](#differentiable-physics-based-simulation)
- [Neural Hair Rendering](#neural-hair-rendering)
- [Semantic Photo Synthesis and Manipulation](#semantic-photo-synthesis-and-manipulation)
- [Texture and Surface Mapping](#texture-and-surface-mapping)
- [Neural Scene Representation and Rendering](#neural-scene-representation-and-rendering)
- [Novel-View Synthesis for Objects and Scenes](#novel-view-synthesis-for-objects-and-scenes)
- [Light, Reflectance, lluminance and Shade](#light--reflectance--lluminance-and-shade)
- [Motion Transfer, Retargeting, Reenactment, Dubbing and Animation](#motion-transfer--retargeting--reenactment--dubbing-and-animation)

## Intruduction of Neural Rendering

**Neural Rendering** is a new and rapidly emerging field that combines generative machine learning techniques with physical knowledge from computer graphics, e.g., by the integration of differentiable rendering into network training. 

Ayush Tewari et. al. define **Neural Rendering** as

> <p align="justify"> <i>Deep image or video generation approaches that enable explicit or implicit control of scene properties such as illumination, camera parameters, pose, geometry, appearance, and semantic structure.</i></p>

A typical neural rendering approach takes as input images corresponding to certain scene conditions (for example, viewpoint, lighting, layout, etc.), builds a “neural” scene representation from them, and “renders” this repre- sentation under novel scene properties to synthesize novel images.

CVPR 2020 tutorial define **Neural Rendering** as
> <p align="justify"> <i>Neural rendering is a new class of deep image and video generation approaches that enable explicit or implicit control of scene properties such as illumination, camera parameters, pose, geometry, appearance, and semantic structure. It combines generative machine learning techniques with physical knowledge from computer graphics to obtain controllable and photo-realistic outputs.</i></p>

Given high-quality scene specifications, **Classic Rendering Methods** can render photorealistic images for a variety of complex real- world phenomena. Moreover, rendering gives us explicit editing control over all the elements of the scene—camera viewpoint, lighting, geometry and materials. However, building high-quality scene models, especially directly from images, requires significant manual effort, and automated scene modeling from images is an open research problem. On the other hand, **Deep Generative Networks** are now starting to produce visually compelling images and videos either from random noise, or conditioned on certain user specifications like scene segmentation and layout. However, they do not yet allow for fine-grained control over scene appearance and cannot always handle the complex, non-local, 3D interactions between scene properties. In contrast, neural rendering methods hold the promise of combining these approaches to enable controllable, high-quality synthesis of novel images from input images/videos. 

**[Differentiable Rendering: A Survey.](https://arxiv.org/abs/2006.12057)**<br>
*Hiroharu Kato, Deniz Beker, Mihai Morariu, Takahiro Ando, Toru Matsuoka, Wadim Kehl, Adrien Gaidon.*<br>

## Related Surveys and Course Notes

**[State of the Art on Neural Rendering.](https://arxiv.org/abs/2004.03805)**<br>
*Ayush Tewari, Ohad Fried, Justus Thies, Vincent Sitzmann, Stephen Lombardi, Kalyan Sunkavalli, Ricardo Martin-Brualla, Tomas Simon, Jason Saragih, Matthias Nießner, Rohit Pandey, Sean Fanello, Gordon Wetzstein, Jun-Yan Zhu, Christian Theobalt, Maneesh Agrawala, Eli Shechtman, Dan B Goldman, Michael Zollhöfer.*<br>
Eurographics 2020.<br>

**[CVPR 2020 tutorial on Neural Rendering.](https://www.neuralrender.com/)**<br>
*Ayush Tewari, Ohad Fried, Justus Thies, Vincent Sitzmann, Stephen Lombardi, Kalyan Sunkavalli, Ricardo Martin-Brualla, Tomas Simon, Jason Saragih, Matthias Nießner, Rohit K. Pandey, Sean Fanello, Gordon Wetzstein, Jun-Yan Zhu, Christian Theobalt, Maneesh Agrawala, Eli Shechtman, Dan B. Goldman, Michael Zollhöfer.*<br>

## Inverse Rendering

**NiLBS: Neural Inverse Linear Blend Skinning.**<br>
*Timothy Jeruzalski, David I.W. Levin, Alec Jacobson, Paul Lalonde, Mohammad Norouzi, Andrea Tagliasacchi.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2004.05980)]

**Learning to Predict 3D Objects with an Interpolation-based Differentiable Renderer.**<br>
*Wenzheng Chen, Jun Gao, Huan Ling, Edward J. Smith, Jaakko Lehtinen, Alec Jacobson, Sanja Fidler.*<br>
NeurIPS 2019. [[PDF](https://arxiv.org/abs/1908.01210)]

**InverseRenderNet: Learning Single Image Inverse Rendering.**<br>
*Ye Yu, William A. P. Smith.*<br>
CVPR 2019. [[PDF](http://openaccess.thecvf.com/content_CVPR_2019/html/Yu_InverseRenderNet_Learning_Single_Image_Inverse_Rendering_CVPR_2019_paper.html)] [[Github](https://github.com/YeeU/InverseRenderNet)] [[IIW Dataset](http://opensurfaces.cs.cornell.edu/publications/intrinsic/#download)] 

**Learning Inverse Rendering of Faces from Real-world Videos.**<br>
*Yuda Qiu, Zhangyang Xiong, Kai Han, Zhongyuan Wang, Zixiang Xiong, Xiaoguang Han.*<br>
arxiv, 2020. [[PDF](https://arxiv.org/abs/2003.12047)] [[Github](https://github.com/RudyQ/InverseFaceRender)]

## Neural Rerendering

Neural Rerendering in the Wild
Moustafa Meshry, Dan B Goldman, Sameh Khamis, Hugues Hoppe, Rohit Pandey, Noah Snavely, Ricardo Martin-Brualla
CVPR 2019. [[](https://arxiv.org/abs/1904.04290)]

## Fluid and Smoke Simulation

**Wave Curves: Simulating Lagrangian water waves on dynamically deforming surfaces.**<br>
*Tomas Skrivan, Andreas Soderstrom, John Johansson, Christoph Sprenger, Ken Museth, [Chris Wojtan](http://pub.ist.ac.at/group_wojtan/index.html).*<br>
ACM Transactions on Graphics (SIGGRAPH 2020). [[PDF](http://pub.ist.ac.at/group_wojtan/projects/2020_Skrivan_WaveCurves/wave_curves_2020.pdf)]

**Constraint Bubbles and Affine Regions: Reduced Fluid Models for Efficient Immersed Bubbles and Flexible Spatial Coarsening.**<br>
*Ryan Goldade, Mridul Aanjaneya, Christopher Batty.*<br>
TOG 2020. [[PDF](https://cs.uwaterloo.ca/~c2batty/papers/Goldade2020/reduced_fluids.pdf)] [[Project](https://cs.uwaterloo.ca/~rgoldade/reducedfluids/)] [[Github](https://github.com/rgoldade/ReducedFluids)]

**Chemomechanical Simulation of Soap Film Flow on Spherical Bubbles.**<br>
*Weizhen Huang, Julian Iseringhausen, Tom Kneiphof, Ziyin Qu, Chenfanfu Jiang, Matthias B. Hullin.*<br>
TOG 2020. [[PDF](https://light.cs.uni-bonn.de/papers/HuangEtAl-SoapBubbles-SIGGRAPH2020.pdf)] [[Project](https://light.cs.uni-bonn.de/chemomechanical-simulation-of-soap-film-flow-on-spherical-bubbles/)] [[Github]()]

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

## Differentiable Physics-Based Simulation

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

## Neural Hair Rendering

**Neural Hair Rendering.**<br>
*[Menglei Chai](mlchai.com), Jian Ren, Sergey Tulyakov.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2004.13297)]

**MichiGAN: Multi-Input-Conditioned Hair Image Generation for Portrait Editing.**<br>
*Zhentao Tan, Menglei Chai, Dongdong Chen, Jing Liao, Qi Chu, Lu Yuan, Sergey Tulyakov, Nenghai Yu.*<br>
SIGGRAPH 2020. [[PDF](https://mlchai.com/files/tan2020michigan.pdf)]

## Semantic Photo Synthesis and Manipulation

**pix2pixHD: High-Resolution Image Synthesis and Semantic Manipulation with Conditional GANs.**<br>
*Ting-Chun Wang, Ming-Yu Liu, Jun-Yan Zhu, Andrew Tao, Jan Kautz, Bryan Catanzaro.*<br>
CVPR 2018. [[PDF](https://arxiv.org/abs/1711.11585)] [[Github](https://github.com/NVIDIA/pix2pixHD)]

**SPADE: Semantic Image Synthesis with Spatially-Adaptive Normalization.**</br>
*Taesung Park, Ming-Yu Liu, Ting-Chun Wang, Jun-Yan Zhu.*<br>
CVPR 2019. [[PDF](https://arxiv.org/abs/1903.07291)] [[Github](https://github.com/NVlabs/SPADE)]

**Semantic Bottleneck Scene Generation.**<br>
*Samaneh Azadi, Michael Tschannen, Eric Tzeng, Sylvain Gelly, Trevor Darrell, Mario Lucic.*<br>
arxiv, 2019. [[PDF](https://arxiv.org/abs/1911.11357)]

**Local Class-Specific and Global Image-Level Generative Adversarial Networks for Semantic-Guided Scene Generation.**<br>
*[Hao Tang](http://disi.unitn.it/~hao.tang/), Dan Xu, Yan Yan, Philip H. S. Torr, [Nicu Sebe](https://scholar.google.com/citations?user=stFCYOAAAAAJ&hl=en).*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/1912.12215)] [[Github](https://github.com/Ha0Tang/LGGAN)]

**SelectionGAN: Multi-Channel Attention Selection GAN with Cascaded Semantic Guidance for Cross-View Image Translation.**<br>
*Hao Tang, Dan Xu, Nicu Sebe, Yanzhi Wang, Jason J. Corso, Yan Yan.*<br>
VPR 2019. [[PDF](https://arxiv.org/abs/1904.06807)] [[Github](https://github.com/Ha0Tang/SelectionGAN)]

## Texture and Surface Mapping

**Wasserstein Generative Models for Patch-based Texture Synthesis.**<br>
*Antoine Houdard, Arthur Leclaire, Nicolas Papadakis, Julien Rabin.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2007.03408)]

**Deep Geometric Texture Synthesis.**<br>
*Amir Hertz, Rana Hanocka, Raja Giryes, Daniel Cohen-Or.*<br>
SIGGRAPH 2020. [[PDF](https://arxiv.org/abs/2007.00074)]

**GramGAN: Deep 3D Texture Synthesis From 2D Exemplars.**<br>
*Tiziano Portenier, Siavash Bigdeli, Orçun Göksel.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2006.16112)]

**GPU-Accelerated Mobile Multi-view Style Transfer.**<br>
*Puneet Kohli, Saravana Gunaseelan, Jason Orozco, Yiwen Hua, Edward Li, Nicolas Dahlquist.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2003.00706v1)]

**Leveraging 2D Data to Learn Textured 3D Mesh Generation.**<br>
*Paul Henderson, Vagia Tsiminaki, Christoph H. Lampert.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.04180)]

**Articulation-aware Canonical Surface Mapping.**<br>
*Nilesh Kulkarni, Abhinav Gupta, David F. Fouhey, Shubham Tulsiani.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.00614)] [[Github](https://github.com/nileshkulkarni/acsm/)] [[Project](https://nileshkulkarni.github.io/acsm/)]

**UnrealText: Synthesizing Realistic Scene Text Images from the Unreal World.**<br>
*Shangbang Long, Cong Yao.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.10608)] [[Github](https://github.com/Jyouhou/UnrealText)]

**Adversarial Texture Optimization from RGB-D Scans.**<br>
*[Jingwei Huang](http://stanford.edu/~jingweih/), [Justus Thies](http://abhijitkundu.info/), [Angela Dai](https://www.3dunderstanding.org/), [Abhijit Kundu](https://justusthies.github.io/), [Chiyu Jiang](https://www.maxjiang.ml/), [Leonidas Guibas](https://geometry.stanford.edu/member/guibas/), [Matthias Nießner](http://www.niessnerlab.org/), [Thomas Funkhouser](https://www.cs.princeton.edu/~funk/).*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.08400)] [[Project](http://stanford.edu/~jingweih/papers/advtex/)] [[Github](https://github.com/hjwdzh/AdversarialTexture)] [[pyRender](https://github.com/hjwdzh/pyRender)]

**CSM: Canonical Surface Mapping via Geometric Cycle Consistency.**<br>
*Nilesh Kulkarni, Abhinav Gupta, Shubham Tulsiani.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1907.10043)] [[Github](https://nileshkulkarni.github.io/csm/)] [[Project](https://nileshkulkarni.github.io/csm/)]

**Texture Mapping for 3D Reconstruction with RGB-D Sensor.**<br>
*Yanping Fu, [Qingan Yan](https://yanqingan.github.io/), Long Yang, Jie Liao, [Chunxia Xiao](http://graphvision.whu.edu.cn/).*<br>
CVPR 2018. [[PDF](https://yanqingan.github.io/docs/cvpr18_texture.pdf)] [[thecvf](http://openaccess.thecvf.com/content_cvpr_2018/papers/Fu_Texture_Mapping_for_CVPR_2018_paper.pdf)] [[Code on Github](https://github.com/fdp0525/G2LTex)]

**Let There Be Color! - Large-Scale Texturing of 3D Reconstructions.**<br>
*Waechter, Michael and Moehrle, Nils and Goesele, Michael.*<br>
ECCV 2018. [[PDF](https://www.gcc.tu-darmstadt.de/media/gcc/papers/Waechter-2014-LTB.pdf)] [[Project](http://www.gcc.tu-darmstadt.de/home/proj/texrecon/)] [[Github](https://github.com/nmoehrle/mvs-texturing)] [[rayint](https://github.com/nmoehrle/rayint)] [[Eigen](http://eigen.tuxfamily.org)] [[Multi-View Environment](http://www.gcc.tu-darmstadt.de/home/proj/mve)] [[mapMAP](http://www.gcc.tu-darmstadt.de/home/proj/mapmap)]

**Learning Category-Specific Mesh Reconstruction from Image Collections.**<br>
*Angjoo Kanazawa, Shubham Tulsiani Alexei A. Efros, Jitendra Malik.*<br>
ECCV 2018. [[Github](akanazawa.github.io/cmr/)] [[Project](https://github.com/akanazawa/cmr)]
 
**Texture Fields: Learning Texture Representations in Function Space.**<br>
*Michael Oechsle, Lars Mescheder, Michael Niemeyer, Thilo Strauss, Andreas Geiger.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1905.07259)]

**AtlasNet: A Papier-Mache Approach to Learning 3D Surface Generation.**<br>
*Thibault Groueix, Matthew Fisher, Vladimir Kim, Bryan Russell, Mathieu Aubry.*<br>
CVPR 2018. [[PDF](https://hal.inria.fr/hal-01718933/file/1802.05384.pdf)] [[Project](http://imagine.enpc.fr/~groueixt/atlasnet/)] [[Github](https://github.com/ThibaultGROUEIX/AtlasNet)]

**Learning Elementary Structures For 3D Shape Generation And Matching.**<br>
*Theo Deprelle, Thibault Groueix, Matthew Fisher, Vladimir G. Kim, Bryan C. Russell, Mathieu Aubry.*<br>
arxiv, 2019. [[PDF](https://arxiv.org/abs/1908.04725)]
[[Project](http://imagine.enpc.fr/~deprellt/atlasnet2/)]
[[Github](https://github.com/TheoDEPRELLE/AtlasNetV2)]

**Learning to Generate Textures on Meshes.**<br>
*Amit Raj, [Cusuh Ham](https://cusuh.github.io/), Connelly Barnes, Vladimir Kim, Jingwan Lu, James Hays.*<br>
CVPR [Deep Generative Models for 3D Understanding 2019](https://sites.google.com/view/3d-widget/) (Best Paper). [[PDF](http://openaccess.thecvf.com/content_cvprw_20/papers/3D-WidDGET/Amit_Raj_Learning_to_Generate_Textures_on_3D_Meshes_CVPRW_2019_paper.pdf)]

**Unsupervised Texture Transfer from Images to Model Collections.**<br>
*[Tuanfeng Yand Wang](http://geometry.cs.ucl.ac.uk/tuanfeng/), [Hao Su](http://ai.ucsd.edu/~haosu/), Qixing Huang, Jingwei Huang, Leonidas J. Guibas, [Niloy J. Mitra](http://www0.cs.ucl.ac.uk/staff/n.mitra/index.html).*<br>
SIGGRAPH Asia 2016. [[PDF](http://ai.ucsd.edu/~haosu/papers/siga16.texture_transfer_small.pdf)]
[[Project](http://geometry.cs.ucl.ac.uk/projects/2016/texture_transfer/)]
[[Data](http://geometry.cs.ucl.ac.uk/tuanfeng/texturetransfer/texture_transfer_code_and_data.zip)]

## Neural Scene Representation and Rendering

**[3D Scene Generation.](https://3dscenegen.github.io/)**<br>
*[Angel X. Chang](https://angelxuanchang.github.io/), [Daniel Ritchie](https://dritchie.github.io/), [Qixing Huang](https://www.cs.utexas.edu/~huangqx/), [Manolis Savva](http://msavva.github.io/).*<br>
CVPR 2019 Workshop.

**Equivariant Neural Rendering.**<br>
*Emilien Dupont, Miguel Angel Bautista, Alex Colburn, Aditya Sankar, Carlos Guestrin, Josh Susskind, Qi Shan.*<br>
ICML 2020. [[PDF](https://arxiv.org/abs/2006.07630)]

**CoReNet: Coherent 3D Scene Reconstruction From a Single RGB Image.**<br>
*Stefan Popov, Pablo Bauszat, Vittorio Ferrari.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2004.12989)]

**Single-View View Synthesis with Multiplane Images.**<br>
*Richard Tucker and Noah Snavely.*<br>
CVPR 2020. [[PDF](https://single-view-mpi.github.io/single_view_mpi.pdf)] [[Project](https://single-view-mpi.github.io/)]

**LIMP: Learning Latent Shape Representations with Metric Preservation Priors.**<br>
*Luca Cosmo, Antonio Norelli, Oshri Halimi, Ron Kimmel, Emanuele Rodolà.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2003.12283)]

**Learning 3D Part Assembly from a Single Image.**<br>
*Yichen Li, Kaichun Mo, Lin Shao, Minhyuk Sung, Leonidas Guibas.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2003.09754)]

**Curriculum DeepSDF.**<br>
*Yueqi Duan, Haidong Zhu, He Wang, Li Yi, Ram Nevatia, Leonidas J. Guibas.*<br>
arxiv, 19 Mar 2020. [[PDF](https://arxiv.org/abs/2003.08593)] [[Github](https://github.com/haidongz-usc/Curriculum-DeepSDF)]

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

**DeepSDF x Sim(3): Extending DeepSDF for automatic 3D shape retrieval and similarity transform estimation.**<br>
*Oladapo Afolabi, Allen Yang, Shankar S. Sastry.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2004.09048)]

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

## Novel-View Synthesis for Objects and Scenes
[Novel-View Synthesis](https://paperswithcode.com/task/novel-view-synthesis/codeless)

**GRAF: Generative Radiance Fields for 3D-Aware Image Synthesis.**<br>
*Katja Schwarz, Yiyi Liao, Michael Niemeyer, Andreas Geiger.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2007.02442)]

**Novel View Synthesis of Dynamic Scenes with Globally Coherent Depths from a Monocular Camera.**<br>
*Jae Shin Yoon, Kihwan Kim, Orazio Gallo, Hyun Soo Park, Jan Kautz.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.01294)]

**Neural Point-Based Graphics.**<br>
*Kara-Ali Aliev, Artem Sevastopolsky, Maria Kolos, Dmitry Ulyanov, Victor Lempitsky.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/1906.08240)] [[Project](https://saic-violet.github.io/npbg/)]

**NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis.**<br>
*[Ben Mildenhall](http://people.eecs.berkeley.edu/~bmild/), [Pratul P. Srinivasan](https://people.eecs.berkeley.edu/~pratul/), [Matthew Tancik](http://www.matthewtancik.com/), [Jonathan T. Barron](https://jonbarron.info/), [Ravi Ramamoorthi](http://cseweb.ucsd.edu/~ravir/), [Ren Ng](https://www2.eecs.berkeley.edu/Faculty/Homepages/yirenng.html).*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2003.08934)] [[Project](http://tancik.com/nerf)] [[Gtihub-Tensorflow](https://github.com/bmild/nerf)] [[krrish94-PyTorch](https://github.com/krrish94/nerf-pytorch)] [[yenchenlin-PyTorch](https://github.com/yenchenlin/nerf-pytorch)]

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

**Self-Supervised 3D Human Pose Estimation via Part Guided Novel Image Synthesis.**<br>
*Jogendra Nath Kundu, Siddharth Seth, Varun Jampani, Mugalodi Rakesh, R. Venkatesh Babu, Anirban Chakraborty.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.04400)]

**IGNOR: Image-guided Neural Object Rendering.**<br>
*Justus Thies, Michael Zollhöfer, Christian Theobalt, Marc Stamminger, [Matthias Nießner](http://niessnerlab.org/publications.html).*<br>
ICLR 2020. arxiv, 26 Nov 2018 (15 Jan 2020). [[PDF](https://arxiv.org/abs/1811.10720)] [[Project](http://niessnerlab.org/projects/thies2020ignor.html)]

**Monocular Neural Image Based Rendering with Continuous View Control.**<br>
*[Xu Chen](https://ait.ethz.ch/people/xu/), [Jie Song](https://ait.ethz.ch/people/song/), Otmar Hilliges.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1901.01880)]

**Extreme View Synthesis.**<br>
*Inchang Choi, Orazio Gallo, Alejandro Troccoli, Min H. Kim, Jan Kautz.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1812.04777)]

**Transformable Bottleneck Networks.**<br>
*Kyle Olszewski, Sergey Tulyakov, Oliver Woodford, Hao Li, Linjie Luo.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Olszewski_Transformable_Bottleneck_Networks_ICCV_2019_paper.pdf)]

**View Independent Generative Adversarial Network for Novel View Synthesis.**<br>
*Xiaogang Xu, Ying-Cong Chen, Jiaya Jia.*<br>
ICCV 2019. [[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Xu_View_Independent_Generative_Adversarial_Network_for_Novel_View_Synthesis_ICCV_2019_paper.pdf)]

## Light, Reflectance, lluminance and Shade

**Enlighten Me: Importance of Brightness and Shadow for Character Emotion and Appeal.**<br>
*Pisut Wisessing, Katja Zibrek, Douglas W. Cunningham, John Dingliana, Rachel McDonnell.*<br>
TOG 2020. [[PDF](https://dl.acm.org/doi/fullHtml/10.1145/3383195)]

**Portrait Shadow Manipulation.**<br>
*[Xuaner Cecilia Zhang](https://people.eecs.berkeley.edu/~cecilia77/), J onathan T. Barron, Yun-Ta Tsai, Rohit Pandey, Xiuming Zhang, Ren Ng, David E. Jacobs.*<br>
SIGGRAPH 2020. [[PDF](https://arxiv.org/abs/2005.08925)] [[Project](https://people.eecs.berkeley.edu/~cecilia77/project-pages/portrait)]

**Lighthouse: Predicting Lighting Volumes for Spatially-Coherent Illumination.**<br>
*Pratul P. Srinivasan, Ben Mildenhall, Matthew Tancik, Jonathan T. Barron, Richard Tucker, Noah Snavely.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.08367)] [GitHub](https://github.com/pratulsrinivasan/lighthouse)] [[Project](https://people.eecs.berkeley.edu/~pratul/lighthouse/)]

**Deep 3D Capture: Geometry and Reflectance from Sparse Multi-View Images.**<br>
*Sai Bi, Zexiang Xu, Kalyan Sunkavalli, David Kriegman, Ravi Ramamoorthi.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.12642)]

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

**Deep Single-Image Portrait Relighting.**<br>
*Hao Zhou, Sunil Hadap, Kalyan Sunkavalli, David W. Jacobs.*<br>
ICCV 2019. [[PDF](https://zhhoper.github.io/paper/zhou_ICCV2019_DPR.pdf)] [[Github](https://github.com/zhhoper/DPR)] [[Project](https://zhhoper.github.io/dpr.html)] [[DPR Dataset](https://drive.google.com/drive/folders/10luekF8vV5vo2GFYPRCe9Rm2Xy2DwHkT?usp=sharing)]

**Single Image Portrait Relighting.**<br>
*[Tiancheng Sun](http://kevinkingo.com/), Jonathan T. Barron, Yun-Ta Tsai, Zexiang Xu, Xueming Yu, Graham Fyffe, Christoph Rhemann, Jay Busch, Paul Debevec, [Ravi Ramamoorthi](https://cseweb.ucsd.edu/~ravir/).*<br> 
SIGGRAPH 2019. [[PDF](https://arxiv.org/abs/1905.00824)]

**Multi-view Relighting using a Geometry-Aware Network.**<br>
*[Julien Philip](https://www-sop.inria.fr/members/Julien.Philip/), [Michael Gharbi](https://research.adobe.com/person/michael-gharbi/), [Tinghui Zhou](https://people.eecs.berkeley.edu/~tinghuiz/), [Alexei (Alyosha) Efros](https://people.eecs.berkeley.edu/~efros/), [George Drettakis](http://www-sop.inria.fr/members/George.Drettakis/).*<br>
SIGGRAPH 2019. [[PDF](https://repo-sam.inria.fr/fungraph/deep-relighting/)]

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

**SfSNet: Learning Shape, Reflectance and llluminance of Faces in the Wild.**<br>
*Soumyadip Sengupta, Angjoo Kanazawa, Carlos D. Castillo, David W. Jacobs.*<br>
CVPR 2018. [[Project](https://senguptaumd.github.io/SfSNet/)] [[PDF](https://arxiv.org/abs/1703.10131)] [[Github](https://github.com/matansel/pix2vertex)]

**Occlusion-aware 3D Morphable Models and an Illumination Prior for Face Image Analysis.**<br>
*Bernhard Egger, Sandro Schoenborn, Andreas Schneider, Adam Kortylewski, Andreas Morel-Forster, Clemens Blumer and Thomas Vetter.*<br>
IJCV 2018. [[BIP Dataset](https://gravis.dmi.unibas.ch/PMM/data/bip/)] [[PDF](http://gravis.dmi.unibas.ch/publications/2018/2018_Egger_IJCV.pdf)]

**DNR: A Neural Rendering Framework for Free-Viewpoint Relighting.**<br>
*Zhang Chen, Anpei Chen, Guli Zhang, Chengyuan Wang, Yu Ji, Kiriakos N. Kutulakos, Jingyi Yu.*<br>
arxiv, 26 Nov 2019. [[PDF](https://arxiv.org/pdf/1911.11530v1.pdf)]

## Motion Transfer, Retargeting, Reenactment, Dubbing and Animation

[[awesome-human-motion](https://github.com/derikon/awesome-human-motion)]

**ReenactNet: Real-time Full Head Reenactment.**<br>
*Mohammad Rami Koujan, Michail Christos Doukas, Anastasios Roussos, Stefanos Zafeiriou.*<br>
FG 2020. [[PDF](https://arxiv.org/abs/2006.10500)]

**FaR-GAN for One-Shot Face Reenactment.**<br>
*Hanxiang Hao, Sriram Baireddy, Amy R. Reibman, Edward J. Delp.*<br>
AI for content creation workshop at CVPR 2020. [[PDF](https://arxiv.org/abs/2005.06402)]

**Skeleton-Aware Networks for Deep Motion Retargeting.**<br>
*Kfir Aberman, Peizhuo Li, Dani Lischinski, Olga Sorkine-Hornung, Daniel Cohen-Or, Baoquan Chen.*<br>
SIGGRAPH 2020. [[Github](https://github.com/DeepMotionEditing/deep-motion-editing)] [[Project](https://deepmotionediting.github.io/retargeting)]

**Unpaired Motion Style Transfer from Video to Animation.**<br>
*Kfir Aberman, Yijia Weng, Dani Lischinski, Daniel Cohen-Or, Baoquan Chen.*<br>
SIGGRAPH 2020. [[Github](https://github.com/DeepMotionEditing/deep-motion-editing)] [[Project](https://deepmotionediting.github.io/style_transfer)]

**MakeItTalk: Speaker-Aware Talking Head Animation.**<br>
*Yang Zhou, DIngzeyu Li, Xintong Han, Evangelos Kalogerakis, Eli Shechtman, Jose Echevarria.*<br>
arriv, 2020. [[PDF](https://arxiv.org/abs/2004.12992)]

**One-Shot Identity-Preserving Portrait Reenactment.**<br>
*Sitao Xiang, Yuming Gu, Pengda Xiang, Mingming He, Koki Nagano, Haiwei Chen, Hao Li.*<br>
arriv, 2020. [[PDF](https://arxiv.org/abs/2004.12452)]

**Neural Head Reenactment with Latent Pose Descriptors.**<br>
*Egor Burkov, Igor Pasechnik, Artur Grigorev, Victor Lempitsky.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.12000)]

**Neural Human Video Rendering by Learning Dynamic Textures and Rendering-to-Video Translation.**<br>
*Lingjie Liu, Weipeng Xu, Marc Habermann, Michael Zollhoefer, Florian Bernard, Hyeongwoo Kim, Wenping Wang, Christian Theobalt.*<br>
arriv, 2020. [[PDF](https://arxiv.org/abs/2001.04947v2)]

**Text-based Editing of Talking-head Video.**<br>
*Ohad Fried, Ayush Tewari, Michael Zollhöfer, Adam Finkelstein, Eli Shechtman, Dan B Goldman Kyle Genova, Zeyu Jin, Christian Theobalt,  Maneesh Agrawala.*<br>
SIGGRAPH 2019. [[PDF](https://www.ohadf.com/projects/text-based-editing/data/text-based-editing.pdf)] [[Project](https://www.ohadf.com/projects/text-based-editing/)]

**StyleRig: Rigging StyleGAN for 3D Control over Portrait Images.**<br>
*A. Tewari, M. Elgharib, G. Bharaj, F. Bernard, H-P. Seidel, P. Perez, M. Zollhöfer, C.Theobalt.*<br>
CVPR 2020. [[PDF](http://gvv.mpi-inf.mpg.de/projects/StyleRig/data/paper.pdf)] [[Project](http://gvv.mpi-inf.mpg.de/projects/StyleRig/)]

**TransMoMo: Invariance-Driven Unsupervised Video Motion Retargeting.**<br>
*Zhuoqian Yang, Wentao Zhu, Wayne Wu, Chen Qian, Qiang Zhou, Bolei Zhou, Chen Change Loy.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2003.14401)] [[Github](https://github.com/yzhq97/transmomo.pytorch)] [[Project](https://yzhq97.github.io/transmomo)]

**Human Motion Transfer from Poses in the Wild.**<br>
*Jian Ren, Menglei Chai, Sergey Tulyakov, Chen Fang, Xiaohui Shen, Jianchao Yang.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2004.03142)]

**First Order Motion Model for Image Animation.**<br>
*[Aliaksandr Siarohin](https://aliaksandrsiarohin.github.io/), [Stéphane Lathuilière](http://stelat.eu/), [Sergey Tulyakov](http://stulyakov.com/), [Elisa Ricci](http://elisaricci.eu/), [Nicu Sebe](http://disi.unitn.it/~sebe/).*<br>
NeurIPS 2019. [[PDF](http://papers.nips.cc/paper/8935-first-order-motion-model-for-image-animation)] [[Project](https://aliaksandrsiarohin.github.io/first-order-model-website)] [[Github](https://github.com/AliaksandrSiarohin/first-order-model)]

**Neural Human Video Rendering: Joint Learning of Dynamic Textures and Rendering-to-Video Translation.**<br>
*Lingjie Liu, Weipeng Xu, Marc Habermann, Michael Zollhoefer, Florian Bernard, Hyeongwoo Kim, Wenping Wang, Christian Theobalt.*<br>
arxiv, 14 Jan 2020. [[PDF](https://arxiv.org/abs/2001.04947)]

**Deferred Neural Rendering: Image Synthesis using Neural.**<br>
*Justus Thies, Michael Zollhöfer, Matthias Nießner.*<br>
SIGGRAPH 2019. [[PDF](https://arxiv.org/abs/1904.12356)]

**LOGAN: Unpaired Shape Transform in Latent Overcomplete Space.**<br>
*Kangxue Yin, Zhiqin Chen, Hui Huang, Daniel Cohen-Or, Hao Zhang.*<br>
SIGGRAPH Asia, 2019. [[PDF](https://arxiv.org/pdf/1903.10170.pdf)]

**Neural Human Video Rendering: Joint Learning of Dynamic Textures and Rendering-to-Video Translation.**<br>
*Lingjie Liu, Weipeng Xu, Marc Habermann, Michael Zollhoefer, Florian Bernard, Hyeongwoo Kim, Wenping Wang, Christian Theobalt.*<br>
arxiv, 14 Jan 2020. [[PDF](https://arxiv.org/abs/2001.04947)]

**FLNet: Landmark Driven Fetching and Learning Network for Faithful Talking Facial Animation Synthesis.**<br>
*Kuangxiao Gu, Yuqian Zhou, Thomas Huang.*<br>
AAAI 2020. [[PDF](https://arxiv.org/abs/1911.09224)] [[GitHub](https://github.com/kgu3/FLNet_AAAI2020)]

**Liquid Warping GAN: A Unified Framework for Human Motion Imitation, Appearance Transfer and Novel View Synthesis.**<br>
*Wen Liu, Zhixin Piao, Jie Min, Wenhan Luo, Lin Ma, Shenghua Gao.*<br>
ICCV 2019. [[PDF](https://arxiv.org/abs/1909.12224)] [[HomePage]( https://motionretargeting2d.github.io)]   [[Github](https://github.com/svip-lab/impersonator)]. 

**Learning Character-Agnostic Motion for Motion Retargeting in 2D.**<br>
*Kfir Aberman, Rundi Wu, Dani Lischinski, Baoquan Chen, Daniel Cohen-Or.*<br>
SIGGRAPH 2019. [[PDF](https://arxiv.org/abs/1905.01680)] [[Github](https://github.com/ChrisWu1997/2D-Motion-Retargeting)] [[Project](https://motionretargeting2d.github.io/)]

**Progressive Pose Attention Transfer for Person Image Generation.**<br>
*Zhen Zhu, Tengteng Huang, Baoguang Shi, Miao Yu, Bofei Wang, Xiang Bai.*<br>
CVPR 2019. [[Project](https://github.com/tengteng95/Pose-Transfer)] [[PDF](https://arxiv.org/abs/1904.03349)]

**Textured Neural Avatars.**<br>
*Aliaksandra Shysheya, Egor Zakharov, Kara-Ali Aliev, Renat Bashirov, Egor Burkov, Karim Iskakov, Aleksei Ivakhnenko, Yury Malkov, Igor Pasechnik, Dmitry Ulyanov, Alexander Vakhitov, Victor Lempitsky.*<br>
CVPR 2019 (oral). [[PDF](https://arxiv.org/abs/1905.08776)] [[Project](https://saic-violet.github.io/texturedavatar/)]

**Appearance Composing GAN: A General Method for Appearance-Controllable Human Video Motion Transfer.**<br>
*Dongxu Wei, Haibin Shen, Kejie Huang.*<br>
arxiv, 25 Nov 2019. [[PDF](https://arxiv.org/abs/1911.10672)]

**EBT: Everybody's Talkin': Let Me Talk as You Want.**<br>
*Linsen Song, [Wayne Wu](http://wywu.github.io/), Chen Qian, [Ran He](https://scholar.google.com/citations?user=ayrg9AUAAAAJ&hl=en), Chen Change Loy.*<br>
arxiv, 15 Jan 2020. [[PDF](https://arxiv.org/abs/2001.05201)] [[Project](https://wywu.github.io/projects/EBT/EBT.html)]

**Photo Wake-Up: 3D Character Animation from a Single Photo.**<br>
*Chung-Yi Weng, Brian Curless, Ira Kemelmacher-Shlizerman.*<br>
CVPR 2019. [[PDF](https://arxiv.org/abs/1812.02246)] [[Project](https://grail.cs.washington.edu/projects/wakeup/)]


## License

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
