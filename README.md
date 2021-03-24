# <p align=center>`awesome neural rendering papers`</p>
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com) [![made-with-Markdown](https://img.shields.io/badge/Made%20with-Markdown-1f425f.svg)](http://commonmark.org)
<!-- [![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](http://ansicolortags.readthedocs.io/?badge=latest) -->

A collection of resources on neural rendering. 

## Contributing

If you think I have missed out on something (or) have any suggestions (papers, implementations and other resources), feel free to [pull a request](https://github.com/xiaweihao/awesome-image-translation/pulls)

Feedback and contributions are welcome!

markdown format:
``` markdown
**Here is the Paper Name.**<br>
*[Author 1](homepage), Author 2, and Author 3.*<br>
Conference or Journal Year. [[PDF](link)] [[Project](link)] [[Github](link)] [[Video](link)] [[Data](link)]
```

## Table of Contents
- [Intruduction of Neural Rendering](#intruduction-of-neural-rendering)
- [Related Surveys and Course Notes](#related-surveys-and-course-notes)
- [Inverse Rendering](#inverse-rendering)
- [Neural Rerendering](#neural-rerendering)
- [Differentiable Rendering](#differentiable-rendering)
- [Volumetric Performance Capture (Free Viewpoint Video)](#volumetric-performance-capture-free-viewpoint-video)
- [Semantic Photo Synthesis and Manipulation](#semantic-photo-synthesis-and-manipulation)
- [Texture and Surface Embedding or Mapping](#texture-and-surface-embedding-or-mapping)
- [Neural Scene Representation and Rendering](#neural-scene-representation-and-rendering)
- [Novel-View Synthesis for Objects and Scenes](#novel-view-synthesis-for-objects-and-scenes)
- [Light, Reflectance, Illuminance and Shade](#light-reflectance-illuminance-and-shade)
- [Dubbing and Talking-Head Animation](#dubbing-and-talking-head-animation)
- [Motion Transfer, Retargeting, and Reenactment](#motion-transfer-retargeting-and-reenactment)

## Intruduction of Neural Rendering

**Neural Rendering** is a new and rapidly emerging field that combines generative machine learning techniques with physical knowledge from computer graphics, e.g., by the integration of differentiable rendering into network training. 

Ayush Tewari et. al. define **Neural Rendering** as

> <p align="justify"> <i>Deep image or video generation approaches that enable explicit or implicit control of scene properties such as illumination, camera parameters, pose, geometry, appearance, and semantic structure.</i></p>

A typical neural rendering approach takes as input images corresponding to certain scene conditions (for example, viewpoint, lighting, layout, etc.), builds a “neural” scene representation from them, and “renders” this representation under novel scene properties to synthesize novel images.

CVPR 2020 tutorial define **Neural Rendering** as
> <p align="justify"> <i>Neural rendering is a new class of deep image and video generation approaches that enable explicit or implicit control of scene properties such as illumination, camera parameters, pose, geometry, appearance, and semantic structure. It combines generative machine learning techniques with physical knowledge from computer graphics to obtain controllable and photo-realistic outputs.</i></p>

Given high-quality scene specifications, **Classic Rendering Methods** can render photorealistic images for a variety of complex real-world phenomena. Moreover, rendering gives us explicit editing control over all the elements of the scene-camera viewpoint, lighting, geometry and materials. However, building high-quality scene models, especially directly from images, requires significant manual effort, and automated scene modeling from images is an open research problem. On the other hand, **Deep Generative Networks** are now starting to produce visually compelling images and videos either from random noise, or conditioned on certain user specifications like scene segmentation and layout. However, they do not yet allow for fine-grained control over scene appearance and cannot always handle the complex, non-local, 3D interactions between scene properties. In contrast, neural rendering methods hold the promise of combining these approaches to enable controllable, high-quality synthesis of novel images from input images/videos. 

## Related Surveys and Course Notes

**[State of the Art on Neural Rendering.](https://arxiv.org/abs/2004.03805)**<br>
*Ayush Tewari, Ohad Fried, Justus Thies, Vincent Sitzmann, Stephen Lombardi, Kalyan Sunkavalli, Ricardo Martin-Brualla, Tomas Simon, Jason Saragih, Matthias Nießner, Rohit Pandey, Sean Fanello, Gordon Wetzstein, Jun-Yan Zhu, Christian Theobalt, Maneesh Agrawala, Eli Shechtman, Dan B Goldman, Michael Zollhöfer.*<br>
Eurographics 2020.<br>

**[CVPR 2020 tutorial on Neural Rendering.](https://www.neuralrender.com/)**<br>
*Ayush Tewari, Ohad Fried, Justus Thies, Vincent Sitzmann, Stephen Lombardi, Kalyan Sunkavalli, Ricardo Martin-Brualla, Tomas Simon, Jason Saragih, Matthias Nießner, Rohit K. Pandey, Sean Fanello, Gordon Wetzstein, Jun-Yan Zhu, Christian Theobalt, Maneesh Agrawala, Eli Shechtman, Dan B. Goldman, Michael Zollhöfer.*<br>

**[Differentiable Rendering: A Survey.](https://arxiv.org/abs/2006.12057)**<br>
*Hiroharu Kato, Deniz Beker, Mihai Morariu, Takahiro Ando, Toru Matsuoka, Wadim Kehl, Adrien Gaidon.*<br>

## Inverse Rendering

**Invertible Neural BRDF for Object Inverse Rendering.**<br>
*Zhe Chen, Shohei Nobuhara, Ko Nishino.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2008.04030)]

**Invertible Neural BRDF for Object Inverse Rendering.**<br>
*Zhe Chen, Shohei Nobuhara, Ko Nishino.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.04030)]

**Inverse Rendering for Complex Indoor Scenes: Shape, Spatially-Varying Lighting and SVBRDF From a Single Image.**<br>
*[Zhengqin Li](http://sites.google.com/a/eng.ucsd.edu/zhengqinli/), [Mohammad Shafiei](https://www.linkedin.com/in/mohammadshafiei/), [Ravi Ramamoorthi](http://cseweb.ucsd.edu/~ravir/), [Kalyan Sunkavalli](http://www.kalyans.org/), [Manmohan Chandraker](http://cseweb.ucsd.edu/~mkchandraker/).*<br>
CVPR 2020.[[PDF](https://drive.google.com/file/d/18zG1kzVpL9XsEVBK95hbpnB-FMlChRXP/view?usp=sharing)] [[Project](http://cseweb.ucsd.edu/~viscomp/projects/CVPR20InverseIndoor/)] [[Github](https://github.com/lzqsd/InverseRenderingOfIndoorScene)]

**Polarimetric Multi-View Inverse Rendering.**<br>
*Jinyu Zhao, Yusuke Monno, Masatoshi Okutomi.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.08830)]

**NiLBS: Neural Inverse Linear Blend Skinning.**<br>
*Timothy Jeruzalski, David I.W. Levin, Alec Jacobson, Paul Lalonde, Mohammad Norouzi, Andrea Tagliasacchi.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2004.05980)]

**Learning to Predict 3D Objects with an Interpolation-based Differentiable Renderer.**<br>
*Wenzheng Chen, Jun Gao, Huan Ling, Edward J. Smith, Jaakko Lehtinen, Alec Jacobson, Sanja Fidler.*<br>
NeurIPS 2019. [[PDF](https://arxiv.org/abs/1908.01210)]

**DRWR: A Differentiable Renderer without Rendering for Unsupervised 3D Structure Learning from Silhouette Images.**<br>
*Zhizhong Han, Chao Chen, Yu-Shen Liu, Matthias Zwicker.*<br>
ICML 2020. [[PDF](https://arxiv.org/abs/2007.06127)]

**InverseRenderNet: Learning Single Image Inverse Rendering.**<br>
*Ye Yu, William A. P. Smith.*<br>
CVPR 2019. [[PDF](http://openaccess.thecvf.com/content_CVPR_2019/html/Yu_InverseRenderNet_Learning_Single_Image_Inverse_Rendering_CVPR_2019_paper.html)] [[Github](https://github.com/YeeU/InverseRenderNet)] [[IIW Dataset](http://opensurfaces.cs.cornell.edu/publications/intrinsic/#download)] 

**Learning Inverse Rendering of Faces from Real-world Videos.**<br>
*Yuda Qiu, Zhangyang Xiong, Kai Han, Zhongyuan Wang, Zixiang Xiong, Xiaoguang Han.*<br>
arxiv, 2020. [[PDF](https://arxiv.org/abs/2003.12047)] [[Github](https://github.com/RudyQ/InverseFaceRender)]

## Neural Rerendering

**Neural Lumigraph Rendering.**<br>
*Petr Kellnhofer, Lars Jebe, Andrew Jones, Ryan Spicer, Kari Pulli, Gordon Wetzstein.*<br>
CVPR 2021. [[PDF](https://arxiv.org/abs/2103.11571)] [[Project](http://www.computationalimaging.org/publications/nlr/)]

**NeRViS: Neural Re-rendering for Full-frame Video Stabilization.**<br>
*[Yu-Lun Liu](https://www.cmlab.csie.ntu.edu.tw/~nothinglo/), [Wei-Sheng Lai](https://www.wslai.net/), [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/), [Yung-Yu Chuang](https://www.csie.ntu.edu.tw/~cyy/), [Jia-Bin Huang](https://filebox.ece.vt.edu/~jbhuang/).*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2102.06205)] [[Github](https://alex04072000.github.io/NeRViS/)]

**Neural Re-Rendering of Humans from a Single Image.**<br>
*Kripasindhu Sarkar, Dushyant Mehta, Weipeng Xu, Vladislav Golyanik, Christian Theobalt.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2101.04104)]

**StyleUV: Diverse and High-fidelity UV Map Generative Model.**<br>
*Myunggi Lee, Wonwoong Cho, Moonheum Kim, David Inouye, Nojun Kwak.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.12893)]

**Neural Rerendering in the Wild.**<br>
*Moustafa Meshry, Dan B Goldman, Sameh Khamis, Hugues Hoppe, Rohit Pandey, Noah Snavely, Ricardo Martin-Brualla.*<br>
CVPR 2019. [[PDF](https://arxiv.org/abs/1904.04290)]

**Revealing Scenes by Inverting Structure from Motion Reconstructions.**<br>
*Francesco Pittaluga, Sanjeev J. Koppal, Sing Bing Kang, Sudipta N. Sinha.*<br>
CVPR 2019. [[PDF](https://arxiv.org/abs/1904.03303)]

## Differentiable Rendering

**Neural Re-Rendering of Humans from a Single Image.**<br>
*Kripasindhu Sarkar, Dushyant Mehta, Weipeng Xu, Vladislav Golyanik, Christian Theobalt.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2101.04104)]

**Modular Primitives for High-Performance Differentiable Rendering.**<br>
*Samuli Laine, Janne Hellsten, Tero Karras, Yeongho Seol, Jaakko Lehtinen, Timo Aila.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.03277)] [[Github](https://github.com/NVlabs/nvdiffrast)]

**Monocular Differentiable Rendering for Self-Supervised 3D Object Detection.**<br>
*Deniz Beker, Hiroharu Kato, Mihai Adrian Morariu, Takahiro Ando, Toru Matsuoka, Wadim Kehl, Adrien Gaidon.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2009.14524)]

## Volumetric Performance Capture (Free Viewpoint Video)

**Monocular Real-Time Volumetric Performance Capture.**<br>
*Ruilong Li, Yuliang Xiu, Shunsuke Saito, Zeng Huang, Kyle Olszewski, Hao Li.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2007.13988)]

**Neural Sparse Voxel Fields.**<br>
*[Lingjie Liu](https://lingjie0206.github.io/), Jiatao Gu, Kyaw Zaw Lin, Tat-Seng Chua, Christian Theobalt.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2007.11571)]

**Volumetric Capture of Humans with a Single RGBD Camera via Semi-Parametric Learning.**<br>
*Rohit Pandey, Anastasia Tkach, Shuoran Yang, Pavel Pidlypenskyi, Jonathan Taylor, Ricardo Martin-Brualla, Andrea Tagliasacchi, George Papandreou, Philip Davidson, Cem Keskin, Shahram Izadi, Sean Fanello.*<br>
CVPR 2019. [[PDF](http://openaccess.thecvf.com/content_CVPR_2019/papers/Pandey_Volumetric_Capture_of_Humans_With_a_Single_RGBD_Camera_via_CVPR_2019_paper.pdf)]

**Neural Volumes: Learning Dynamic Renderable Volumes from Images.**<br>
*Stephen Lombardi, Tomas Simon, Jason Saragih, Gabriel Schwartz, Andreas Lehrmann, Yaser Sheikh.*<br>
SIGGRAPH 2019. [[PDF](https://arxiv.org/abs/1906.07751)]

## Semantic Photo Synthesis and Manipulation

**StyleFlow: Attribute-conditioned Exploration of StyleGAN-Generated Images using Conditional Continuous Normalizing Flows.**<br>
*Rameen Abdal, Peihao Zhu, Niloy Mitra, Peter Wonka.*<br>
Siggraph Asia 2020. [[PDF](https://arxiv.org/abs/2008.02401)] [[Github](https://rameenabdal.github.io/StyleFlow)]

**Layered Neural Rendering for Retiming People in Video.**<br>
*Erika Lu, Forrester Cole, Tali Dekel, Weidi Xie, Andrew Zisserman, David Salesin, William T. Freeman, Michael Rubinstein.*<br>
SIGGRAPH Asia 2020. [[PDF](https://arxiv.org/abs/2009.07833)] [[Project](https://retiming.github.io/)]

**Neural Hair Rendering.**<br>
*[Menglei Chai](mlchai.com), Jian Ren, Sergey Tulyakov.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2004.13297)]

**MichiGAN: Multi-Input-Conditioned Hair Image Generation for Portrait Editing.**<br>
*Zhentao Tan, Menglei Chai, Dongdong Chen, Jing Liao, Qi Chu, Lu Yuan, Sergey Tulyakov, Nenghai Yu.*<br>
SIGGRAPH 2020. [[PDF](https://mlchai.com/files/tan2020michigan.pdf)]

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

## Texture and Surface Embedding or Mapping

**NeuTex: Neural Texture Mapping for Volumetric Neural Rendering.**<br>
*Fanbo Xiang, Zexiang Xu, Miloš Hašan, Yannick Hold-Geoffroy, Kalyan Sunkavalli, Hao Su.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2103.00762)]

**Better Patch Stitching for Parametric Surface Reconstruction.**<br>
*Zhantao Deng, Jan Bednařík, Mathieu Salzmann, Pascal Fua.*<br>
3DV 2020. [[PDF](https://arxiv.org/abs/2010.07021)]

**Continuous Surface Embeddings.**<br>
*Natalia Neverova, David Novotny, Marc Szafraniec, Vasil Khalidov, Patrick Labatut, Andrea Vedaldi.*<br>
NerIPS 2020. [[PDF](https://arxiv.org/abs/2011.12438)]

**Transposer: Universal Texture Synthesis Using Feature Maps as Transposed Convolution Filter.**<br>
*Guilin Liu, Rohan Taori, Ting-Chun Wang, Zhiding Yu, Shiqiu Liu, Fitsum A. Reda, Karan Sapra, Andrew Tao, Bryan Catanzaro.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2007.07243)]

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

[[Awesome Neural Radiance Fields](https://github.com/yenchenlin/awesome-NeRF)]

[[NeRF Explosion 2020](https://dellaert.github.io/NeRF/)]

**DONeRF: Towards Real-Time Rendering of Neural Radiance Fields using Depth Oracle Networks.**<br>
*Thomas Neff, Pascal Stadlbauer, Mathias Parger, Andreas Kurz, Chakravarty R. Alla Chaitanya, Anton Kaplanyan, Markus Steinberger.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2103.03231)] [[Project](https://depthoraclenerf.github.io/)]

**Mixture of Volumetric Primitives for Efficient Neural Rendering.**<br>
*Stephen Lombardi, Tomas Simon, Gabriel Schwartz, Michael Zollhoefer, Yaser Sheikh, Jason Saragih.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2103.01954)]

**ShaRF: Shape-conditioned Radiance Fields from a Single View.**<br>
*Konstantinos Rematas, Ricardo Martin-Brualla, Vittorio Ferrari.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2102.08860)] [[Project](http://www.krematas.com/sharf/index.html)]

**NeRF--: Neural Radiance Fields Without Known Camera Parameters.**<br>
*Zirui Wang, Shangzhe Wu, [Weidi Xie](https://weidixie.github.io/weidi-personal-webpage/), [Min Chen](https://sites.google.com/site/drminchen/home), [Victor Adrian Prisacariu](https://eng.ox.ac.uk/people/victor-prisacariu/).*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2102.07064)] [[Project](http://nerfmm.active.vision/)]

**A-NeRF: Surface-free Human 3D Pose Refinement via Neural Rendering.**<br>
*[Shih-Yang Su](https://lemonatsu.github.io/), [Frank Yu](https://yu-frank.github.io/), [Michael Zollhoefer](https://zollhoefer.com/), [Helge Rhodin](http://helge.rhodin.de/).*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2102.06199)] [[Project](https://lemonatsu.github.io/ANeRF-Surface-free-Pose-Refinement/)]

**Neural Geometric Level of Detail: Real-time Rendering with Implicit 3D Shapes.**<br>
*Towaki Takikawa, Joey Litalien, Kangxue Yin, Karsten Kreis, Charles Loop, Derek Nowrouzezahrai, Alec Jacobson, Morgan McGuire, Sanja Fidler.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2101.10994)]

**Neural Volume Rendering: NeRF And Beyond.**<br>
*Frank Dellaert, Lin Yen-Chen.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2101.05204)]

**Non-line-of-Sight Imaging via Neural Transient Fields.**<br>
*Siyuan Shen, Zi Wang, Ping Liu, Zhengqing Pan, Ruiqian Li, Tian Gao, Shiying Li, Jingyi Yu.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2101.00373)]

**DeepSurfels: Learning Online Appearance Fusion.**<br>
*Marko Mihajlovic, Silvan Weder, Marc Pollefeys, Martin R. Oswald.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2012.14240)]

**Non-Rigid Neural Radiance Fields: Reconstruction and Novel View Synthesis of a Deforming Scene from Monocular Video.**<br>
*Edgar Tretschk, Ayush Tewari, Vladislav Golyanik, Michael Zollhöfer, Christoph Lassner, Christian Theobalt.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.12247)] [[Project](https://gvv.mpi-inf.mpg.de/projects/nonrigid_nerf/)] [[Github](https://github.com/facebookresearch/nonrigid_nerf)]

**Learned Initializations for Optimizing Coordinate-Based Neural Representations.**<br>
*[Matthew Tancik](https://www.matthewtancik.com/), [[Ben Mildenhall](https://people.eecs.berkeley.edu/~bmild/), Terrance Wang, Divi Schmidt, Pratul P. Srinivasan, [Jonathan T. Barron](https://jonbarron.info/), [Ren Ng](https://www2.eecs.berkeley.edu/Faculty/Homepages/yirenng.html).*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.02189)] [[Project](https://www.matthewtancik.com/learnit)]

**Learning Compositional Radiance Fields of Dynamic Human Heads.**<br>
*Ziyan Wang, Timur Bagautdinov, Stephen Lombardi, Tomas Simon, Jason Saragih, Jessica Hodgins, Michael Zollhöfer.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.09955)]

**OSF: Object-Centric Neural Scene Rendering.**<br>
*Michelle Guo, Alireza Fathi, Jiajun Wu, Thomas Funkhouser.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.08503)] [[Project](https://shellguo.com/osf)]

**Deformed Implicit Field: Modeling 3D Shapes with Learned Dense Correspondence.**<br>
*Yu Deng, Jiaolong Yang, Xin Tong.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.13650)]

**Iso-Points: Optimizing Neural Implicit Surfaces with Hybrid Representations.**<br>
*Wang Yifan, Shihao Wu, Cengiz Oztireli, Olga Sorkine-Hornung.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.06434)]

**Dynamic Neural Radiance Fields for Monocular 4D Facial Avatar Reconstruction.**<br>
*Guy Gafni, Justus Thies, Michael Zollhöfer, Matthias Nießner.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.03065)] [[Project](https://gafniguy.github.io/4D-Facial-Avatars/)] [[Video](https://youtu.be/m7oROLdQnjk)]

**Portrait Neural Radiance Fields from a Single Image.**<br>
*Chen Gao, Yichang Shih, Wei-Sheng Lai, Chia-Kai Liang, Jia-Bin Huang.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.05903)] [[Project](https://portrait-nerf.github.io/)]

**iNeRF: Inverting Neural Radiance Fields for Pose Estimation.**<br>
*[Lin Yen-Chen](http://yenchenlin.me/), Pete Florence, Jonathan T. Barron, Alberto Rodriguez, Phillip Isola, Tsung-Yi Lin.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.05877)] [[Project](http://yenchenlin.me/inerf/)]

**NeRV: Neural Reflectance and Visibility Fields for Relighting and View Synthesis.**<br>
*Pratul P. Srinivasan, Boyang Deng, Xiuming Zhang, Matthew Tancik, Ben Mildenhall, Jonathan T. Barron.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.03927)] [[Project](https://people.eecs.berkeley.edu/~pratul/nerv)]

**pixelNeRF: Neural Radiance Fields from One or Few Images.**<br>
*Alex Yu, Vickie Ye, Matthew Tancik, Angjoo Kanazawa.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.02190)] [[Project](https://alexyu.net/pixelnerf)]

**AutoInt: Automatic Integration for Fast Neural Volume Rendering.**<br>
*David B. Lindell, Julien N. P. Martel, Gordon Wetzstein.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.01714)]

**Space-time Neural Irradiance Fields for Free-Viewpoint Video.**<br>
*Wenqi Xian, Jia-Bin Huang, Johannes Kopf, Changil Kim.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.12950)] [[Project](https://video-nerf.github.io/)]

**DeRF: Decomposed Radiance Fields.**<br>
*Daniel Rebain, Wei Jiang, Soroosh Yazdani, Ke Li, Kwang Moo Yi, Andrea Tagliasacchi.*<br>
CVPR 2021. [[PDF](https://arxiv.org/abs/2011.12490)] [[Project](https://ubc-vision.github.io/derf/)]

**D-NERF: Deformable Neural Radiance Fields.**<br>
*Keunhong Park, Utkarsh Sinha, Jonathan T. Barron, Sofien Bouaziz, Dan B Goldman, Steven M. Seitz, Ricardo-Martin Brualla.*<br>
CVPR 2021. [[PDF](https://arxiv.org/abs/2011.12948)] [[Project](https://nerfies.github.io/)]

**GIRAFFE: Representing Scenes as Compositional Generative Neural Feature Fields.**<br>
*Michael Niemeyer, Andreas Geiger.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.12100)]

**Neural Unsigned Distance Fields for Implicit Function Learning.**<br>
*Julian Chibane, Aymen Mir, Gerard Pons-Moll.*<br>
NeurIPS 2020. [[PDF](https://arxiv.org/abs/2010.13938)] [[Github](https://virtualhumans.mpi-inf.mpg.de/ndf/)]

**GRF: Learning a General Radiance Field for 3D Scene Representation and Rendering.**<br>
*[Alex Trevithick](https://alextrevithick.github.io/), [Bo Yang](https://yang7879.github.io/).*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2010.04595)] [[Github](https://github.com/alextrevithick/GRF)]

**[3D Scene Generation.](https://3dscenegen.github.io/)**<br>
*[Angel X. Chang](https://angelxuanchang.github.io/), [Daniel Ritchie](https://dritchie.github.io/), [Qixing Huang](https://www.cs.utexas.edu/~huangqx/), [Manolis Savva](http://msavva.github.io/).*<br>
CVPR 2019 Workshop.

**Local Deep Implicit Functions for 3D Shape.**<br>
*Kyle Genova, Forrester Cole, Avneesh Sud, Aaron Sarna, Thomas Funkhouser.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/1912.06126)]

**PatchNets: Patch-Based Generalizable Deep Implicit 3D Shape Representations.**<br>
*Edgar Tretschk, Ayush Tewari, Vladislav Golyanik, Michael Zollhöfer, Carsten Stoll, Christian Theobalt.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.01639)]

**Unsupervised 3D Learning for Shape Analysis via Multiresolution Instance Discrimination.**<br>
*Peng-Shuai Wang, Yu-Qi Yang, Qian-Fang Zou, Zhirong Wu, Yang Liu, Xin Tong.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.01068)]

**Learning Implicit Fields for Generative Shape Modeling.**<br>
*Zhiqin Chen, Hao Zhang.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/1812.02822)] [[Project](https://www.sfu.ca/~zhiqinc/imgan/Readme.html)] [[Github](https://github.com/czq142857/implicit-decoder)]

**Geometric Correspondence Fields: Learned Differentiable Rendering for 3D Pose Refinement in the Wild.**<br>
*Alexander Grabner, Yaming Wang, Peizhao Zhang, Peihong Guo, Tong Xiao, Peter Vajda, Peter M. Roth, Vincent Lepetit.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.08939)]

**Equivariant Neural Rendering.**<br>
*[Emilien Dupont](https://emiliendupont.github.io/), Miguel Angel Bautista, [Alex Colburn](https://www.colburn.org/), Aditya Sankar, [Carlos Guestrin](https://homes.cs.washington.edu/~guestrin/), Josh Susskind, [Qi Shan](http://shanqi.github.io/).*<br>
ICML 2020. [[PDF](https://arxiv.org/abs/2006.07630)] [[Github](https://github.com/apple/ml-equivariant-neural-rendering)]

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

**Neural Scene Graphs for Dynamic Scenes.**<br>
*Julian Ost, Fahim Mannan, Nils Thuerey, Julian Knodt, Felix Heide.*<br>
CVPR 2021. [[PDF](https://arxiv.org/abs/2011.10379)] [[Project](https://light.princeton.edu/neural-scene-graphs/)]

## Novel-View Synthesis for Objects and Scenes

[Novel-View Synthesis](https://paperswithcode.com/task/novel-view-synthesis/codeless)

### Implicit Neural Representations or Neural Radiance Fields

**DyNeRF: Neural 3D Video Synthesis.**<br>
*Tianye Li, Mira Slavcheva, Michael Zollhoefer, Simon Green, Christoph Lassner, Changil Kim, Tanner Schmidt, Steven Lovegrove, Michael Goesele, Zhaoyang Lv.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2103.02597)] [[Project](https://neural-3d-video.github.io/)]

**ID-Unet: Iterative Soft and Hard Deformation for View Synthesis.**<br>
*Mingyu Yin, Li Sun, Qingli Li.*<br>
CVPR 2021. [[PDF](https://arxiv.org/abs/2103.02264)]

**Neural Radiance Flow for 4D View Synthesis and Video Processing.**<br>
*Yilun Du, Yinan Zhang, Hong-Xing Yu, Joshua B. Tenenbaum, Jiajun Wu.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.09790)] [[Project](https://yilundu.github.io/nerflow/)]

**Neural Body: Implicit Neural Representations with Structured Latent Codes for Novel View Synthesis of Dynamic Humans.**<br>
*Sida Peng, Yuanqing Zhang, Yinghao Xu, Qianqian Wang, Qing Shuai, Hujun Bao, Xiaowei Zhou.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2012.15838)] [[Project](https://zju3dv.github.io/neuralbody/)]

**NSFF: Neural Scene Flow Fields for Space-Time View Synthesis of Dynamic Scenes.**<br>
*Zhengqi Li, Simon Niklaus, Noah Snavely, Oliver Wang.*<br>
CVPR 2021. [[PDF](https://arxiv.org/abs/2011.13084)] [[Project](http://www.cs.cornell.edu/~zl548/NSFF)]

**NeRF++: Analyzing and Improving Neural Radiance Fields.**<br>
*Kai Zhang, Gernot Riegler, Noah Snavely, Vladlen Koltun.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2010.07492)] [[Github](https://github.com/Kai-46/nerfplusplus)]

**X-Fields: Implicit Neural View-, Light- and Time-Image Interpolation.**<br>
*MOJTABA BEMANA, KAROL MYSZKOWSKI, HANS-PETER SEIDEL, TOBIAS RITSCHEL.*<br>
Siggraph Asia 2020. [[PDF](http://xfields.mpi-inf.mpg.de/paper/X_Fields__siggasia_2020.pdf)]

**NeRF in the Wild: Neural Radiance Fields for Unconstrained Photo Collections.**<br>
*Ricardo Martin-Brualla, Noha Radwan, Mehdi S. M. Sajjadi, Jonathan T. Barron, Alexey Dosovitskiy, Daniel Duckworth.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.02268)] [[Github](https://nerf-w.github.io/)]

**pixelNeRF: Neural Radiance Fields from One or Few Images.**<br>
*Alex Yu, Vickie Ye, Matthew Tancik, Angjoo Kanazawa.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.02190)] [[Project](https://alexyu.net/pixelnerf/)] [[Github](https://github.com/sxyu/pixel-nerf)]

**GRAF: Generative Radiance Fields for 3D-Aware Image Synthesis.**<br>
*Katja Schwarz, Yiyi Liao, Michael Niemeyer, Andreas Geiger.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2007.02442)]

**NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis.**<br>
*[Ben Mildenhall](http://people.eecs.berkeley.edu/~bmild/), [Pratul P. Srinivasan](https://people.eecs.berkeley.edu/~pratul/), [Matthew Tancik](http://www.matthewtancik.com/), [Jonathan T. Barron](https://jonbarron.info/), [Ravi Ramamoorthi](http://cseweb.ucsd.edu/~ravir/), [Ren Ng](https://www2.eecs.berkeley.edu/Faculty/Homepages/yirenng.html).*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2003.08934)] [[Project](http://tancik.com/nerf)] [[Gtihub-Tensorflow](https://github.com/bmild/nerf)] [[krrish94-PyTorch](https://github.com/krrish94/nerf-pytorch)] [[yenchenlin-PyTorch](https://github.com/yenchenlin/nerf-pytorch)]

### From Single Image

**Generative View Synthesis: From Single-view Semantics to Novel-view Images.**<br>
*Tewodros Habtegebrial, Varun Jampani, Orazio Gallo, Didier Stricker.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.09106)] [[Project](https://gvsnet.github.io/)]

**ShaRF: Shape-conditioned Radiance Fields from a Single View.**<br>
*Konstantinos Rematas, Ricardo Martin-Brualla, Vittorio Ferrari.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2102.08860)] [[Project](http://www.krematas.com/sharf/index.html)]

**Worldsheet: Wrapping the World in a 3D Sheet for View Synthesis from a Single Image.**<br>
*[Ronghang Hu](https://ronghanghu.com/), [Deepak Pathak](https://www.cs.cmu.edu/~dpathak/).*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.09854)] [[Project](https://worldsheet.github.io/)]

**Unsupervised Novel View Synthesis from a Single Image.**<br>
*Pierluigi Zama Ramirez, Alessio Tonioni, Federico Tombari.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2102.03285)]

**Infinite Nature: Perpetual View Generation of Natural Scenes from a Single Image.**<br>
*Andrew Liu, Richard Tucker, Varun Jampani, Ameesh Makadia, Noah Snavely, Angjoo Kanazawa.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.09855)]

### Others

**Nex: Real-time View Synthesis with Neural Basis Expansion.**<br>
*S. Wizadwongsa, P. Phongthawee, J. Yenphraphai, S. Suwajanakorn.*<br>
CVPR 2021 (oral). [[PDF](https://arxiv.org/abs/2103.05606)]

**Bowtie Networks: Generative Modeling for Joint Few-Shot Recognition and Novel-View Synthesis.**<br>
*Zhipeng Bao, Yu-Xiong Wang, Martial Hebert.*<br>
ICLR 2021. [[PDF](https://openreview.net/pdf?id=ESG-DMKQKsD)]

**IBRNet: Learning Multi-View Image-Based Rendering.**<br>
*Qianqian Wang, Zhicheng Wang, Kyle Genova, Pratul Srinivasan, Howard Zhou, Jonathan T. Barron, Ricardo Martin-Brualla, Noah Snavely, Thomas Funkhouser.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2102.13090)]

**SVS: Stable View Synthesis.**<br>
*Gernot Riegler, Vladlen Koltun.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.07233)] [[Github](https://github.com/intel-isl/StableViewSynthesis)] [[Video](https://youtu.be/gqgXIY09htI)]

**FVS: Free View Synthesis.**<br>
*Gernot Riegler, [Vladlen Koltun](http://vladlen.info).*<br>
ECCV 2020. [[PDF](http://vladlen.info/papers/FVS.pdf)]  [[Code&Data](https://github.com/intel-isl/FreeViewSynthesis)]

**Deep View Synthesis via Self-Consistent Generative Network.**<br>
*Zhuoman Liu, Wei Jia, Ming Yang, Peiyao Luo, Yong Guo, Mingkui Tan.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2101.10844)]

**Novel View Synthesis via Depth-guided Skip Connections.**<br>
*Yuxin Hou, Arno Solin, Juho Kannala.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2101.01619)]

**Vid2Actor: Free-viewpoint Animatable Person Synthesis from Video in the Wild.**<br>
*Chung-Yi Weng, Brian Curless, Ira Kemelmacher-Shlizerman.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.12884)] [[Project](https://grail.cs.washington.edu/projects/vid2actor/)] [[Video](https://youtu.be/Zec8Us0v23o)]

**Object-Centric Neural Scene Rendering.**<br>
*Michelle Guo, Alireza Fathi, Jiajun Wu, Thomas Funkhouser.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.08503)] [[Project](https://shellguo.com/osf)]

**RGBD-Net: Predicting Color and Depth Images for Novel Views Synthesis.**<br>
*Phong Nguyen, Animesh Karnewar, Lam Huynh, Esa Rahtu, Jiri Matas, Janne Heikkila.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.14398)]

**Rotationally-Temporally Consistent Novel-View Synthesis of Human Performance Video.**<br> 
*Youngjoong Kwon, Stefano Petrangeli, Dahun Kim, Haoliang Wang, Eunbyung Park, Viswanathan Swaminathan, Henry Fuchs.*<br>
ECCV 2020. [[pdf](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123490375.pdf)] [[Supplement](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123490375-supp.zip)]

**A Recurrent Transformer Network for Novel View Action Synthesis.**<br> 
*Kara Marie Schatz, Erik Quintanilla, Shruti Vyas, Yogesh S Rawat.*<br>
ECCV 2020. [[pdf](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123720409.pdf)] [[Supplement](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123720409-supp.zip)]

**MatryODShka: Real-time 6DoF Video View Synthesis using Multi-Sphere Images.**<br> 
*Benjamin Attal, Selena Ling, Aaron Gokaslan, Christian Richardt, James Tompkin.*<br>
ECCV 2020. [[pdf](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123460426.pdf)] [[Supplement](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123460426-supp.zip)]

**Novel View Synthesis on Unpaired Data by Conditional Deformable Variational Auto-Encoder.**<br> 
*Mingyu Yin, Li Sun, Qingli Li.*<br>
ECCV 2020. [[pdf](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123730086.pdf)] [[Supplement](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123730086-supp.pdf)]

**Deep Multi Depth Panoramas for View Synthesis.**<br>
*Kai-En Lin, Zexiang Xu, Ben Mildenhall, Pratul P. Srinivasan, Yannick Hold-Geoffroy, Stephen DiVerdi, Qi Sun, Kalyan Sunkavalli, Ravi Ramamoorthi.*<br>
ECCV 2020. [[pdf](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123580324.pdf)] [[Supplement](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123580324-supp.zip)]

**Semantic View Synthesis.**</br>
*[Hsin-Ping Huang](https://hhsinping.github.io/), [Hung-Yu Tseng](https://sites.google.com/site/hytseng0509/), [Hsin-Ying Lee](http://vllab.ucmerced.edu/hylee/), [Jia-Bin Huang](https://filebox.ece.vt.edu/~jbhuang/).*</br>
ECCV 2020. [[PDF](hhsinping.github.io/svs/link/paper.pdf)] [[Project](hhsinping.github.io/svs/index.htm)]  

**Deep Multi Depth Panoramas for View Synthesis.**<br>
*Kai-En Lin, Zexiang Xu, Ben Mildenhall, Pratul P. Srinivasan, Yannick Hold-Geoffroy, Stephen DiVerdi, Qi Sun, Kalyan Sunkavalli, Ravi Ramamoorthi.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2008.01815)]

**Unsupervised Continuous Object Representation Networks for Novel View Synthesis.**<br>
*Nicolai Häni, Selim Engin, Jun-Jee Chao, Volkan Isler.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2007.15627)]

**AUTO3D: Novel View Synthesis Through Unsupervisely Learned Variational Viewpoint and Global 3D Representation.**<br>
*Xiaofeng Liu, Tong Che, Yiqun Lu, Chao Yang, Site Li, Jane You.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2007.06620)]

**A Free Viewpoint Portrait Generator with Dynamic Styling.**<br>
*Anpei Chen, Ruiyang Liu, Ling Xie, Jingyi Yu.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2007.03780)]

**Novel View Synthesis of Dynamic Scenes with Globally Coherent Depths from a Monocular Camera.**<br>
*Jae Shin Yoon, Kihwan Kim, Orazio Gallo, Hyun Soo Park, Jan Kautz.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.01294)]

**Neural Point-Based Graphics.**<br>
*Kara-Ali Aliev, Artem Sevastopolsky, Maria Kolos, Dmitry Ulyanov, Victor Lempitsky.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/1906.08240)] [[Project](https://saic-violet.github.io/npbg/)]

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

## Light, Reflectance, Illuminance and Shade

**DSRN: an Efficient Deep Network for Image Relighting.**<br>
*Sourya Dipta Das, Nisarg A. Shah, Saikat Dutta, Himanshu Kumar.*<br>
arxiv 2021. [[PDF](https://arxiv.org/abs/2102.09242)]

**Relightable 3D Head Portraits from a Smartphone Video.**<br>
*Artem Sevastopolsky, Savva Ignatiev, Gonzalo Ferrer, Evgeny Burnaev, Victor Lempitsky.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.09963)] [[Project](https://saic-violet.github.io/relightable-portrait/)] [[Video](https://www.youtube.com/watch?v=qQnNalM9hgY)]

**NeRD: Neural Reflectance Decomposition from Image Collections.**<br>
*[Mark Boss](https://markboss.me), [Raphael Braun](https://uni-tuebingen.de/en/fakultaeten/mathematisch-naturwissenschaftliche-fakultaet/fachbereiche/informatik/lehrstuehle/computergrafik/lehrstuhl/mitarbeiter/raphael-braun/), [Varun Jampani](https://varunjampani.github.io/), [Jonathan T. Barron](https://jonbarron.info/), [Ce Liu](http://people.csail.mit.edu/celiu/), [Hendrik P. A. Lensch](https://uni-tuebingen.de/en/faculties/faculty-of-science/departments/computer-science/lehrstuehle/computergrafik/computer-graphics/staff/prof-dr-ing-hendrik-lensch/).*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.03918)] [[Project](https://markboss.me/publication/2021-nerd/)] [[Github](https://github.com/cgtuebingen/NeRD-Neural-Reflectance-Decomposition)]

**Deferred Neural Lighting: Free-viewpoint Relighting from Unstructured Photographs.**<br>
*[Duan Gao](https://gao-duan.github.io/), [Guojun Chen](https://www.microsoft.com/en-us/research/people/guoch/), [Yue Dong](http://yuedong.shading.me/), [Pieter Peers](http://www.cs.wm.edu/~ppeers/), [Kun Xu](https://cg.cs.tsinghua.edu.cn/people/~kun/), [Xin Tong](http://www.xtong.info/).*<br>
ACM Transactions on Graphics (Proceedings of SIGGRAPH Asia 2020)

**Cross-Camera Convolutional Color Constancy.**<br>
*Mahmoud Afifi, Jonathan T. Barron, Chloe LeGendre, Yun-Ta Tsai, Francois Bleibel.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.11890)]

**Towards Geometry Guided Neural Relighting with Flash Photography.**<br>
*Di Qiu, Jin Zeng, Zhanghan Ke, Wenxiu Sun, Chengxi Yang.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.05157v1)]

**Light Stage Super-Resolution: Continuous High-Frequency Relighting.**<br>
*Tiancheng Sun, Zexiang Xu, Xiuming Zhang, Sean Fanello, Christoph Rhemann, Paul Debevec, Yun-Ta Tsai, Jonathan T. Barron, Ravi Ramamoorthi.*<br>
Siggraph Asia 2020. [[PDF](https://arxiv.org/abs/2010.08888)]

**Neural Light Transport for Relighting and View Synthesis.**<br>
*Xiuming Zhang, Sean Fanello, Yun-Ta Tsai, Tiancheng Sun, Tianfan Xue, Rohit Pandey, Sergio Orts-Escolano, Philip Davidson, Christoph Rhemann, Paul Debevec, Jonathan T. Barron, Ravi Ramamoorthi, William T. Freeman.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.03806)] [[Project](http://nlt.csail.mit.edu/)]

**NuI-Go: Recursive Non-Local Encoder-Decoder Network for Retinal Image Non-Uniform Illumination Removal.**<br>
*Chongyi Li, Huazhu Fu, Runmin Cong, Zechao Li, Qianqian Xu.*<br>
ACM MM 2020. [[PDF](https://arxiv.org/abs/2008.02984)]

**Learning to Factorize and Relight a City.**<br>
*Andrew Liu, Shiry Ginosar, Tinghui Zhou, Alexei A. Efros, Noah Snavely.*<br>
ECCV 2020. [[PDF](https://arxiv.org/abs/2008.02796)] [[Project](http://factorize-a-city.github.io/)]

**Object-based Illumination Estimation with Rendering-aware Neural Networks.**<br>
*Xin Wei, Guojun Chen, Yue Dong, Stephen Lin, Xin Tong.*<br>
ECCV 2200. [[PDF](https://arxiv.org/abs/2008.02514)]

**Learning Illumination from Diverse Portraits.**<br>
*Chloe LeGendre, Wan-Chun Ma, Rohit Pandey, Sean Fanello, Christoph Rhemann, Jason Dourgarian, Jay Busch, Paul Debevec.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.02396)]

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
arxiv 2019. [[PDF](https://arxiv.org/pdf/1911.11530v1.pdf)]

**Deep Illumination: Approximating Dynamic Global Illumination with Generative Adversarial Network.**<br>
*Manu Mathew Thomas, Angus G. Forbes.*<br>
arxiv 2017. [[PDF](https://arxiv.org/abs/1710.09834)]

**Deep Shading: Convolutional Neural Networks for Screen-Space Shading.**<br>
*Oliver Nalbach, Elena Arabadzhiyska, Dushyant Mehta, Hans-Peter Seidel, Tobias Ritschel.*<br>
arixv 2016. [[PDF](https://arxiv.org/abs/1603.06078)]

**One Shot Radiance: Global Illumination Using Convolutional Autoencoders.**<br>
*Giulio Jiang, Bernhard Kainz.*<br>
arxiv 2019. [[PDF](https://arxiv.org/abs/1910.02480)]

## Dubbing and Talking-Head Animation

**HeadGAN: Video-and-Audio-Driven Talking Head Synthesis.**<br>
*Michail Christos Doukas, Stefanos Zafeiriou, Viktoriia Sharmanska.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.08261)]

**DECA: Learning an Animatable Detailed 3D Face Model from In-The-Wild Images.**<br>
*Yao Feng, Haiwen Feng, Michael J. Black, Timo Bolkart.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.04012)] [[Github](https://github.com/YadiraF/DECA)]

**One-Shot Free-View Neural Talking-Head Synthesis for Video Conferencing.**<br>
*Ting-Chun Wang, Arun Mallya, Ming-Yu Liu.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.15126)] [[Project](https://nvlabs.github.io/face-vid2vid)]

**Large-Scale Multilingual Audio Visual Dubbing.**<br>
*Yi Yang, Brendan Shillingford, Yannis Assael, Miaosen Wang, Wendi Liu, Yutian Chen, Yu Zhang, Eren Sezener, Luis C. Cobo, Misha Denil, Yusuf Aytar, Nando de Freitas.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.03530)] [[Video](https://www.youtube.com/playlist?list=PLSi232j2ZA6_1Exhof5vndzyfbxAhhEs5)]

**MakeItTalk: Speaker-Aware Talking-Head Animation.**<br>
*Yang Zhou, Xintong Han, Eli Shechtman, Jose Echevarria, Evangelos Kalogerakis, Dingzeyu Li.*<br>
SIGGRAPH Asia 2020. [[PDF](https://arxiv.org/abs/2004.12992)] [[Github](https://github.com/adobe-research/MakeItTalk)]

**EBT: Everybody's Talkin': Let Me Talk as You Want.**<br>
*Linsen Song, [Wayne Wu](http://wywu.github.io/), Chen Qian, [Ran He](https://scholar.google.com/citations?user=ayrg9AUAAAAJ&hl=en), Chen Change Loy.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2001.05201)] [[Project](https://wywu.github.io/projects/EBT/EBT.html)]

**FLNet: Landmark Driven Fetching and Learning Network for Faithful Talking Facial Animation Synthesis.**<br>
*Kuangxiao Gu, Yuqian Zhou, Thomas Huang.*<br>
AAAI 2020. [[PDF](https://arxiv.org/abs/1911.09224)] [[GitHub](https://github.com/kgu3/FLNet_AAAI2020)]

**Text-based Editing of Talking-head Video.**<br>
*Ohad Fried, Ayush Tewari, Michael Zollhöfer, Adam Finkelstein, Eli Shechtman, Dan B Goldman Kyle Genova, Zeyu Jin, Christian Theobalt,  Maneesh Agrawala.*<br>
SIGGRAPH 2019. [[PDF](https://www.ohadf.com/projects/text-based-editing/data/text-based-editing.pdf)] [[Project](https://www.ohadf.com/projects/text-based-editing/)]

**Speech Driven Talking Face Generation from a Single Image and an Emotion Condition.**<br>
*Sefik Emre Eskimez, You Zhang, Zhiyao Duan.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.03592)]

## Motion Transfer, Retargeting, and Reenactment

[[awesome-human-motion](https://github.com/derikon/awesome-human-motion)]

**Local Motion Phases for Learning Multi-Contact Character Movements.**<br>
*[Sebastian Starke](https://www.linkedin.com/in/sebastian-starke-b281a6148/), Yiwei Zhao, Taku Komura, Kazi Zaman.*<br>
Siggraph 2020. [[PDF](https://github.com/sebastianstarke/AI4Animation/blob/master/Media/SIGGRAPH_2020/Paper.pdf)] [[AI4Animation](https://github.com/sebastianstarke/AI4Animation)]

**Neural State Machine for Character-Scene Interactions.**<br>
*Sebastian Starke, He Zhang, Taku Komura, Jun Saito.*<br>
Siggraph Asia 2019. [[PDF](https://github.com/sebastianstarke/AI4Animation/blob/master/Media/SIGGRAPH_Asia_2019/Paper.pdf)] [[Code & Data](https://github.com/sebastianstarke/AI4Animation/blob/master/AI4Animation/SIGGRAPH_Asia_2019)]

**High-Fidelity Neural Human Motion Transfer from Monocular Video.**<br>
*Moritz Kappel, Vladislav Golyanik, Mohamed Elgharib, Jann-Ole Henningson, Hans-Peter Seidel, Susana Castillo, Christian Theobalt, Marcus Magnor.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.10974)] [[Project](https://graphics.tu-bs.de/publications/kappel2020high-fidelity)] 

**Single-Shot Freestyle Dance Reenactment.**<br>
*Oran Gafni, Oron Ashual, Lior Wolf.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2012.01158)]

**Image Animation with Perturbed Masks.**<br>
*Yoav Shalev, Lior Wolf.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2011.06922)] [[Github](https://github.com/itsyoavshalev/Image-Animation-with-Perturbed-Masks)]

**Photorealistic Audio-driven Video Portraits.**<br>
*Xin Wen, Miao Wang, Christian Richardt, Ze-Yin Chen, Shi-Min Hu.*<br>
TVCG (ISMAR 2020). [[PDF](https://richardt.name/publications/audio-dvp/AudioDVP-WenEtAl-TVCG2020.pdf)] [[Github](https://github.com/xinwen-cs/AudioDVP)] [[Project](https://richardt.name/publications/audio-dvp/)]

**FACEGAN: Facial Attribute Controllable rEenactment GAN.**<br>
*Soumya Tripathy, Juho Kannala, Esa Rahtu.*<br>
WACV 2021. [[PDF](https://arxiv.org/abs/2011.04439)]

**Generative Adversarial Networks in Human Emotion Synthesis:A Review.**<br>
*Noushin Hajarolasvadi, Miguel Arjona Ramírez, Hasan Demirel.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2010.15075)]

**Mesh Guided One-shot Face Reenactment using Graph Convolutional Networks.**<br>
*Guangming Yao, Yi Yuan, Tianjia Shao, Kun Zhou.*<br>
ACM MM 2020. [[PDF](https://arxiv.org/abs/2008.07783)]

**Learning to Generate Diverse Dance Motions with Transformer.**<br>
*Jiaman Li, Yihang Yin, Hang Chu, Yi Zhou, Tingwu Wang, Sanja Fidler, Hao Li.*<br>
arxiv 2020. [[PDF](https://arxiv.org/abs/2008.08171)]

**Action2Motion: Conditioned Generation of 3D Human Motions.**<br>
*Chuan Guo, Xinxin Zuo, Sen Wang, Shihao Zou, Qingyao Sun, Annan Deng, Minglun Gong, Li Cheng.*<br>
ACM MultiMedia 2020. [[PDF](https://arxiv.org/abs/2007.15240)]

**MEAD: A Large-scale Audio-visual Dataset for Emotional Talking Face Generation.**<br>
*Kaisiyuan Wang, Qianyi Wu, Linsen Song, Zhuoqian Yang, Wayne Wu, Chen Qian, Ran He, Yu Qiao, Chen Change Loy.*<br>
ECCV 2020. [[PDF](https://wywu.github.io/)] [[Github](https://wywu.github.io/)] [[Project](https://wywu.github.io/)]

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

**LipGAN: Towards Automatic Face-to-Face Translation.**<br>
*Prajwal K R, Rudrabha Mukhopadhyay, Jerin Philip, Abhishek Jha, Vinay Namboodiri, C.V. Jawahar.*<br>
ACM MM 2019. [[PDF](https://arxiv.org/abs/2003.00418v1)] [[Github](https://github.com/Rudrabha/LipGAN)]

**One-Shot Identity-Preserving Portrait Reenactment.**<br>
*Sitao Xiang, Yuming Gu, Pengda Xiang, Mingming He, Koki Nagano, Haiwei Chen, Hao Li.*<br>
arriv, 2020. [[PDF](https://arxiv.org/abs/2004.12452)] 

**Neural Head Reenactment with Latent Pose Descriptors.**<br>
*Egor Burkov, Igor Pasechnik, Artur Grigorev, Victor Lempitsky.*<br>
CVPR 2020. [[PDF](https://arxiv.org/abs/2004.12000)]

**Neural Human Video Rendering by Learning Dynamic Textures and Rendering-to-Video Translation.**<br>
*Lingjie Liu, Weipeng Xu, Marc Habermann, Michael Zollhoefer, Florian Bernard, Hyeongwoo Kim, Wenping Wang, Christian Theobalt.*<br>
arriv, 2020. [[PDF](https://arxiv.org/abs/2001.04947v2)]

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
arxiv 2020. [[PDF](https://arxiv.org/abs/2001.04947)]

**Deferred Neural Rendering: Image Synthesis using Neural.**<br>
*Justus Thies, Michael Zollhöfer, Matthias Nießner.*<br>
SIGGRAPH 2019. [[PDF](https://arxiv.org/abs/1904.12356)]

**LOGAN: Unpaired Shape Transform in Latent Overcomplete Space.**<br>
*Kangxue Yin, Zhiqin Chen, Hui Huang, Daniel Cohen-Or, Hao Zhang.*<br>
SIGGRAPH Asia, 2019. [[PDF](https://arxiv.org/pdf/1903.10170.pdf)]

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
arxiv 2019. [[PDF](https://arxiv.org/abs/1911.10672)]

## License

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
