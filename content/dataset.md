# Image Translation, Restoration, Enhancement Datasets.

A list of image translation, restoration and enhancement datasets.

## Image Translation

See the [scripts](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix/blob/master/docs/datasets.md) to download related datasets.

### Image_Harmonization
* IDH [[Homepage](https://github.com/bcmi/Image_Harmonization_Datasets)] [[PDF](https://arxiv.org/pdf/1911.13239.pdf)]
* [DeepHarmonization](http://vllab.ucmerced.edu/ytsai/CVPR17/real_data.zip)
* [colorRealism](http://balaton.graphics.cs.cmu.edu/jlalonde/colorStatistics/db.zip)
* [Dataset](http://efrosprojects.eecs.berkeley.edu/realism/human_evaluation.zip) for Realism Prediction.
* [Dataset](http://efrosprojects.eecs.berkeley.edu/realism/color_adjustment.zip) for Color Adjustment.

## Image Enhancemnt
### HDR
* Deep-SR-ITM [[Train](https://drive.google.com/open?id=144QYC403NrFXunlsr4k8MXUCxrlauVYH)] [[Test](https://drive.google.com/open?id=144QYC403NrFXunlsr4k8MXUCxrlauVYH)]
   * Joint Learning of Super-Resolution and Inverse Tone-Mapping for 4K UHD HDR Applications. [[PDF](https://arxiv.org/abs/1904.11176)] [[Supplementary Material](https://drive.google.com/open?id=1bijPrcN-ont-iP0-DqyhBta_rj3dmZEe)] [[Github](https://github.com/sooyekim/Deep-SR-ITM)] Soo Ye Kim, Jihyong Oh, Munchurl Kim.  ICCV 2019.

* MIT-Adobe FiveK Dataset [[Download, 50GB](https://data.csail.mit.edu/graphics/fivek/)]

* HDR+Burst Photography Dataset [[PDF](http://static.googleusercontent.com/media/www.hdrplusdata.org/en//hdrplus.pdf)] [[Download](https://www.hdrplusdata.org/dataset.html)] Small Version: 153 images, 37GB; Full: 3640, 765GB.

* The Laval Indoor HDR Dataset [[PDF](http://vision.gel.ulaval.ca/~jflalonde/projects/deepIndoorLight/)] [[Homepage](http://indoor.hdrdb.com/)]

* SICE [[PDF]](https://ieeexplore.ieee.org/document/8259342) [[Github]](https://github.com/csjcai/SICE)
   * A large-scale multi-exposure image dataset, which contains 589 elaborately selected high-resolution multi-exposure sequences with 4,413 images. 
   * SICE: Learning a Deep Single Image Contrast Enhancer from Multi-Exposure Images. TIP 2018
* Funt HDR Dataset [[Homepage]](http://www.cs.sfu.ca/~colour/data/funt_hdr/#DATA)
* Stanford DHR Dataset [[Homepage]](http://scarlet.stanford.edu/~brian/hdr/hdr.html)
* DML-HDR Dataset [[Homepage]](http://dml.ece.ubc.ca/data/DML-HDR/)
* Deep High Dynamic Range Imaging of Dynamic Scenes [[Homepage]](ucsd.edu/~viscomp/projects/SIG17HDR/)
* HDR-eye Dataset [[Homepage]](https://mmspg.epfl.ch/hdr-eye)
* sIBL Dataset [[Homepage]](http://www.hdrlabs.com/sibl/archive/downloads/) Free HDRI sets for smart Image-Based Lighting.
* Fairchild Dataset [[Homepage]](http://www.cis.rit.edu/fairchild/HDRPS/EXRs/)
* City Scene Panorama Dataset.
* EMPA HDR Dataset [[Homepage]](http://empamedia.ethz.ch/)
* pfstools HDR image Gallery [[Homepage]](http://pfstools.sourceforge.net/resources.html) 
* sIBL Archive Dataset [[Homepage]](http://www.hdrlabs.com/sibl/)
* SGA17_testset [[Download](http://hdrv.org/hdrcnn/material/sga17_testset.zip)

### Quality Enhancement
* DPED Dataset [[PDF]](https://arxiv.org/pdf/1704.02470.pdf)[[Project]](http://dped-photos.vision.ee.ethz.ch/) [[Homeage]](http://people.ee.ethz.ch/~ihnatova/) [[Github]](https://github.com/aiff22/DPED).
   * DPED: DSLR-Quality Photos on Mobile Devices with Deep Convolutional Networks. Andrey Ignatov, Nikolay Kobyshev, Radu Timofte, Kenneth Vanhoey, Luc Van Gool. ICCV 2017.
* WESPE Dataset [[PDF]](https://arxiv.org/pdf/1709.01118.pdf) [[Project]](http://people.ee.ethz.ch/~ihnatova/wespe.html) 
   * Photos from several common smartphones (iPhone 3GS, BlackBerry Passport, Sony Xperia Z; iPhone 6, Huawei P9, HTC One M9, Meizu M3s, Xiaomi Redmi 3X and Nexus 5X.)
   * WESPE: Weakly Supervised Photo Enhancer for Digital Cameras. 
 Andrey Ignatov, Nikolay Kobyshev, Radu Timofte, Kenneth Vanhoey, Luc Van Gool.

### Low-Light [Research](https://zhuanlan.zhihu.com/p/78297097)
 * IIW Dataset (EnlightenGAN) [[Github](https://github.com/TAMU-VITA/EnlightenGAN)]
 * A Dataset of Multi-Illumination Images in the Wild. [[GitHub](http://t.cn/AiD5VknV)]
 * OpenCE [[Github]](https://github.com/baidut/OpenCE)
 * VIP-LowLight Dataset [[Project]](https://uwaterloo.ca/vision-image-processing-lab/research-demos/vip-lowlight-dataset)
   * Eight Natural Images Captured in Very Low-Light Conditions, Audrey Chung.
 * ReNOIR [[PDF]](https://arxiv.org/abs/1409.8230) [[Project]](http://ani.stat.fsu.edu/~abarbu/Renoir.html)
   * RENOIR - A Dataset for Real Low-Light Image Noise Reduction (JVCIR2018), Josue Anaya, Adrian Barbu
 * Raw Image Low-Light Object Dataset [[Project]](https://wiki.qut.edu.au/display/cyphy/Datasets)
   * Dan Richards, James Sergeant, Michael Milford, Peter Corke.
 * Learning to See in the Dark [[PDF]](http://openaccess.thecvf.com/content_cvpr_2018/papers/Chen_Learning_to_See_CVPR_2018_paper.pdf) [[Project]](http://vladlen.info/publications/learning-see-dark/)
   * Learning to See in the Dark (CVPR2018), Chen Chen, Qifeng Chen, Jia Xu, Vladlen Koltun.
 * ExDARK [[PDF]](https://arxiv.org/abs/1805.11227)
   * Getting to Know Low-light Images with The Exclusively Dark Dataset. Yuen Peng Loh, Chee Seng Chan.
   
### Color-Enhancement

 * MIT FiveK dataset [[PDF]](https://people.csail.mit.edu/sparis/publi/2011/cvpr_auto/Bychkovsky_11_Learning_Photo_Adjustment.pdf) [[Project]](https://data.csail.mit.edu/graphics/fivek/)
   * Learning Photographic Global Tonal Adjustment with a Database of Input / Output Image Pairs (CVPR2011), Vladimir Bychkovsky, Sylvain Paris and Eric Chan, Fredo Durand.
 * LRAICE-Dataset [[PDF]](https://www.cv-foundation.org/openaccess/content_cvpr_2014/papers/Yan_A_Learning-to-Rank_Approach_2014_CVPR_paper.pdf) [[Project]]() 
   * A Learning-to-Rank Approach for Image Color Enhancement (CVPR2014), Jianzhou Yan, Stephen Lin, Sing Bing Kang, Xiaoou Tang.
 * DPED dataset [[PDF]](https://arxiv.org/abs/1704.02470) [[Project]](http://people.ee.ethz.ch/~ihnatova/)
   * DSLR-quality photos on mobile devices with deep convolutional networks (ICCV2017), A. Ignatov, N. Kobyshev, K. Vanhoey, R. Timofte, L. Van Gool.
 * The 500px Dataset [[PDF]](https://www.microsoft.com/en-us/research/uploads/prod/2018/01/Exposure.pdf) 
   * Exposure: A White-Box Photo Post-Processing Framework (TOG2018), Yuanming Hu, Hao He, Chenxi Xu, Baoyuan Wang, Stephen Lin.
   
### Underwater Image Enhancement
 * [UIEB: An Underwater Image Enhancement Benchmark Dataset and Beyond.](li-chongyi.github.io/proj_benchmark.html) [[arXiv](https://arxiv.org/pdf/1901.05495.pdf)] [[TIP](https://ieeexplore.ieee.org/document/8917818)]
 * [Underwater Scene Prior Inspired Deep Underwater Image and Video Enhancement.](https://li-chongyi.github.io/proj_underwater_image_synthesis.html)

## Image Restoration

### Image-Inpainting
 * Image Inpainting [[Project]](http://chalearnlap.cvc.uab.es/dataset/30/description/)
   * 2018 Chalearn Looking at People Satellite Workshop ECCV

### Image Denoising
 * Smartphone Image Denoising Dataset [[PDF]](http://openaccess.thecvf.com/content_cvpr_2018/papers/Abdelhamed_A_High-Quality_Denoising_CVPR_2018_paper.pdf)
   * A High-Quality Denoising Dataset for Smartphone Cameras (CVPR2018), Abdelrahman Abdelhamed, Stephen Lin, Michael S. Brown.
 * Darmstadt Noise Dataset [[PDF]](https://download.visinf.tu-darmstadt.de/papers/2017-cvpr-ploetz-benchmarking_denoising_algorithms-preprint.pdf) [[Project]](https://noise.visinf.tu-darmstadt.de/)
   * Benchmarking Denoising Algorithms with Real Photographs (CVPR2017), Tobias Plötz and Stefan Roth.
 * PolyU Dataset [[PDF]](https://arxiv.org/pdf/1804.02603.pdf) [[Project]](https://github.com/csjunxu/PolyU-Real-World-Noisy-Images-Dataset)
   * Real-world Noisy Image Denoising: A New Benchmark (Arxiv2017), Jun Xu, Hui Li, Zhetong Liang, David Zhang, and Lei Zhang.
 * RENOIR Dataset [[PDF]](https://arxiv.org/pdf/1409.8230.pdf) [[Project]](http://ani.stat.fsu.edu/~abarbu/Renoir.html)
   * A Dataset for Real Low-Light Image Noise Reduction (Arxiv2014), J. Anaya, A. Barbu. 
 * Holistic Dataset [[PDF]](http://snam.ml/assets/ccnoise_cvpr16/ccnoise_cvpr16.pdf) [[Project]](http://snam.ml/research/ccnoise)
   * A Holistic Approach to Cross-Channel Image Noise Modeling and its Application to Image Denoising (CVPR2016), Seonghyeon Nam, Youngbae Hwang, Yasuyuki Matsushita, Seon Joo Kim.
   
### Super-Resolution and Up-Sampling
 * Train91 [[PDF]](http://www.columbia.edu/~jw2966/papers/YWHM10-TIP.pdf) [[Project]](http://www.ifp.illinois.edu/~jyang29/ScSR.htm)
   * Image Super-Resolution via Sparse Representation (TIP2010), Jianchao Yang, John Wright, Thomas Huang, and Yi Ma.
 * Set5 [[PDF]](http://www.vision.ee.ethz.ch/~timofter/publications/Timofte-ICCV-2013.pdf) [[Project]](http://www.vision.ee.ethz.ch/~timofter/ICCV2013_ID1774_SUPPLEMENTARY/index.html)
   * Anchored Neighborhood Regression for Fast Example-Based Super-Resolution (ICCV2013), Radu Timofte, Vincent De Smet, and Luc Van Gool.
 * Set14 [[PDF]](http://www.cs.technion.ac.il/~elad/publications/conferences/2010/ImageScaleUp_LNCS.pdf)
   * On Single Image Scale-Up Using Sparse-Representations (International conference on curves and surfaces 2010), Zeyde, Roman and Elad, Michael and Protter, Matan.
 * B100 [[PDF]](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/papers/amfm_pami2010.pdf) [[Project]](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/resources.html)
   * Contour Detection and Hierarchical Image Segmentation (TPAMI2011), P. Arbelaez, M. Maire, C. Fowlkes and J. Malik.
 * Urban100 [[PDF]](https://uofi.box.com/shared/static/8llt4ijgc39n3t7ftllx7fpaaqi3yau0.pdf) [[Project]](https://sites.google.com/site/jbhuang0604/publications/struct_sr)
   * Single Image Super-Resolution from Transformed Self-Exemplars (CVPR2015), Jia-Bin Huang, Abhishek Singh, and Narendra Ahuja.
 * DIV2K [[PDF]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8014884) [[Project]](https://data.vision.ee.ethz.ch/cvl/DIV2K/)
   * NTIRE 2017 Challenge on Single Image Super-Resolution: Dataset and Study (CVPRW2017), Eirikur Agustsson, Radu Timofte.
 * LIVE [[PDF]](https://ieeexplore.ieee.org/document/1709988) [[Project]](http://live.ece.utexas.edu/research/quality/subjective.htm)
   * A Statistical Evaluation of Recent Full Reference Image Quality Assessment Algorithms (TIP2006), H.R. Sheikh, M.F. Sabir and A.C. Bovik.
 * Super-Resolution Erlangen (SupER) [[PDF]](https://arxiv.org/pdf/1709.04881.pdf) [[Project]](https://superresolution.tf.fau.de/)
   * Benchmarking Super-Resolution Algorithms on Real Data (Arxiv2017), Thomas Köhler, Michel Bätz, Farzad Naderi, André Kaup, Andreas Maier, and Christian Riess.     

### Dehazing
 * Waterloo IVC Dehazed Image Database [[PDF]](http://ieeexplore.ieee.org/document/7351475/) [[Project]](http://ivc.uwaterloo.ca/database/Dehaze/Dehaze-Database.php)
   * Perceptual evaluation of single image dehazing algorithms (ICIP'15), Kede Ma, Wentao Liu and Zhou Wang.
 * FRIDA dataset [[Project]](http://perso.lcpc.fr/tarel.jean-philippe/bdd/frida.html)
 * D-hazy [[PDF]](http://www.meo.etc.upt.ro/AncutiProjectPages/D_Hazzy_ICIP2016/D_HAZY_ICIP2016.pdf) [[Project]](http://www.meo.etc.upt.ro/AncutiProjectPages/D_Hazzy_ICIP2016/)
 * CHIC [[PDF]](https://link.springer.com/chapter/10.1007/978-3-319-33618-3_12)
   * A Color Image Database for Haze Model and Dehazing Methods Evaluation
 * HazeRD [[PDF]](https://ieee-dataport.org/documents/hazerd-outdoor-dataset-dehazing-algorithms)
   * HazeRD: an outdoor dataset for dehazing algorithms
 * I-HAZE : a dehazing benchmark with real hazy and haze-free outdoor images [[PDF]](https://arxiv.org/abs/1804.05091)
 * O-HAZE : a dehazing benchmark with real hazy and haze-free out
 door images [[PDF]](https://arxiv.org/abs/1804.05101)
 * RESIDE: A Benchmark for Single Image Dehazing [[Project]](https://sites.google.com/view/reside-dehaze-datasets)

### Deblurring (sharpening)
 * Understanding and evaluating blind deconvolution algorithms (CVPR'09) [[PDF]](https://ieeexplore.ieee.org/document/5206815)
 * Edge-based blur kernel estimation using patch priors [[PDF]](https://ieeexplore.ieee.org/document/6528301/)
 * Benchmarking blind deconvolution with a real-world database (ECCV'12) [[PDF]](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.379.1398&rep=rep1&type=pdf)
 * A Comparative Study for Single Image Blind Deblurring (CVPR'16) [[Project]](http://vllab.ucmerced.edu/wlai24/cvpr16_deblur_study/)

### De-raining

#### Rain streak removal
##### Single image deraining
 * Rain Streak Database  [[DATASET]](http://www1.cs.columbia.edu/CAVE/projects/rain_ren/rain_ren.php)[[PDF]](http://www1.cs.columbia.edu/CAVE/publications/pdfs/Garg_TOG06.pdf)
   * Photorealistic rendering of rain streaks
 * Rain12 [[DATASET]](http://yu-li.github.io/paper/li_cvpr16_rain.zip)[[PDF]](https://ieeexplore.ieee.org/abstract/document/7934436/)
   * Single Image Rain Streak Decomposition Using Layer Priors
 * Rain100L and Rain100H [[DATASET]](http://www.icst.pku.edu.cn/struct/Projects/joint_rain_removal.html)[[PDF](https://ieeexplore.ieee.org/document/8099666)]
   * Deep Joint Rain Detection and Removal From a Single Image
 * Rain800 [[DATASET](https://github.com/hezhangsprinter/ID-CGAN)][[PDF](https://arxiv.org/abs/1701.05957)]
   * ID_CGAN:Image De-raining Using a Conditional Generative Adversarial Network
 * Rain1400 [[DATASET](https://xueyangfu.github.io/projects/cvpr2017.html)][[PDF](http://openaccess.thecvf.com/content_cvpr_2017/papers/Fu_Removing_Rain_From_CVPR_2017_paper.pdf)]
   * Removing rain from single images via a deep detail network
 * Rain1200 [[DATASET]](https://github.com/hezhangsprinter/DID-MDN)[[PDF](https://arxiv.org/abs/1802.07412)]
   * Density-aware Single Image De-raining using a Multi-stream Dense Network
 * Heavy Rain Dataset [[DATASET](https://drive.google.com/file/d/1rFpW_coyxidYLK8vrcfViJLDd-BcSn4B/view)][[PDF](http://export.arxiv.org/pdf/1904.05050)]
   * Heavy Rain Image Restoration: Integrating Physics Model and Conditional Adversarial Learning
 * SPANet Dataset [[DATASET](https://stevewongv.github.io/derain-project.html)][[PDF](https://arxiv.org/pdf/1904.01538.pdf)]
   * Spatial Attentive Single-Image Deraining with a High Quality Real Rain Dataset

##### Video rain removal
* MS-CSC-Rain-Streak-Removal [[Project]](https://github.com/MinghanLi/MS-CSC-Rain-Streak-Removal)
   * Video Rain Streak Removal By Multiscale ConvolutionalSparse Coding

#### Rain drop removal

* Attentive Generative Adversarial Network for Raindrop Removal from A Single Image (CVPR'18) [[Project]](https://rui1996.github.io/raindrop/raindrop_removal.html)


## Generate Synthetic Datasets

[Generating Training Data for Denoising Real RGB Images via Camera Pipeline Simulation.](https://arxiv.org/abs/1904.08825) 
Ronnachai Jaroensri, Camille Biscarrat, Miika Aittala, Frédo Durand. [GitHub](https://github.com/12dmodel/camera_sim), 2019.

[Meta-Sim: Learning to Generate Synthetic Datasets.](https://arxiv.org/abs/1904.11621) [Github](https://nv-tlabs.github.io/meta-sim/), ICCV 2019. 

