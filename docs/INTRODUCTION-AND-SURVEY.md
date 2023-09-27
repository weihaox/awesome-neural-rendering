## Intruduction of Neural Rendering

**Neural Rendering** is a new and rapidly emerging field that combines generative machine learning techniques with physical knowledge from computer graphics, e.g., by the integration of differentiable rendering into network training. 

Ayush Tewari et. al. define **Neural Rendering** as

> <p align="justify"> <i>Deep image or video generation approaches that enable explicit or implicit control of scene properties such as illumination, camera parameters, pose, geometry, appearance, and semantic structure.</i></p>

A typical neural rendering approach takes as input images corresponding to certain scene conditions (for example, viewpoint, lighting, layout, etc.), builds a “neural” scene representation from them, and “renders” this representation under novel scene properties to synthesize novel images.

CVPR 2020 tutorial define **Neural Rendering** as
> <p align="justify"> <i>Neural rendering is a new class of deep image and video generation approaches that enable explicit or implicit control of scene properties such as illumination, camera parameters, pose, geometry, appearance, and semantic structure. It combines generative machine learning techniques with physical knowledge from computer graphics to obtain controllable and photo-realistic outputs.</i></p>

Given high-quality scene specifications, **Classic Rendering Methods** can render photorealistic images for a variety of complex real-world phenomena. Moreover, rendering gives us explicit editing control over all the elements of the scene-camera viewpoint, lighting, geometry and materials. However, building high-quality scene models, especially directly from images, requires significant manual effort, and automated scene modeling from images is an open research problem. On the other hand, **Deep Generative Networks** are now starting to produce visually compelling images and videos either from random noise, or conditioned on certain user specifications like scene segmentation and layout. However, they do not yet allow for fine-grained control over scene appearance and cannot always handle the complex, non-local, 3D interactions between scene properties. In contrast, neural rendering methods hold the promise of combining these approaches to enable controllable, high-quality synthesis of novel images from input images/videos. 

## Related Surveys and Course Notes

**[Advances in Neural Rendering.](https://arxiv.org/abs/2111.05849)**<br>
*Ayush Tewari\*, Justus Thies\*, Ben Mildenhall\*, Pratul Srinivasan\*, Edgar Tretschk, Yifan Wang, Christoph Lassner, Vincent Sitzmann, Ricardo Martin-Brualla, Stepehen Lombardi, Tomas Simon, Christian Theobalt, Matthias Niessner, Jonathan T. Barron, Gordon Wetzstein, Michael Zollhoefer, and Vladislav Golyanik.*<br>
Eurographics State-of-the-Art Report 2022.

**[Advances in Neural Rendering.](https://arxiv.org/abs/2111.05849)**<br>
*Ayush Tewari, Justus Thies, Ben Mildenhall, Pratul Srinivasan, Edgar Tretschk, Yifan Wang, Christoph Lassner, Vincent Sitzmann, Ricardo Martin-Brualla, Stephen Lombardi, Tomas Simon, Christian Theobalt, Matthias Niessner, Jonathan T. Barron, Gordon Wetzstein, Michael Zollhoefer, Vladislav Golyanik.*<br>
ACM SIGGRAPH 2021 Courses.

**[State of the Art on Neural Rendering.](https://arxiv.org/abs/2004.03805)**<br>
*Ayush Tewari, Ohad Fried, Justus Thies, Vincent Sitzmann, Stephen Lombardi, Kalyan Sunkavalli, Ricardo Martin-Brualla, Tomas Simon, Jason Saragih, Matthias Nießner, Rohit Pandey, Sean Fanello, Gordon Wetzstein, Jun-Yan Zhu, Christian Theobalt, Maneesh Agrawala, Eli Shechtman, Dan B Goldman, Michael Zollhöfer.*<br>
Eurographics 2020.<br>

**[Advances in Neural Rendering.](https://www.neuralrender.com/)**<br>
*Ayush Tewari, Ohad Fried, Justus Thies, Vincent Sitzmann, Stephen Lombardi, Kalyan Sunkavalli, Ricardo Martin-Brualla, Tomas Simon, Jason Saragih, Matthias Nießner, Rohit K. Pandey, Sean Fanello, Gordon Wetzstein, Jun-Yan Zhu, Christian Theobalt, Maneesh Agrawala, Eli Shechtman, Dan B. Goldman, Michael Zollhöfer.*<br>
SIGGRAPH 2021 Course/CVPR 2020 Tutorial.

**[Nerfstudio: A Modular Framework for Neural Radiance Field Development.](https://docs.nerf.studio/en/latest/)**<br>
*Matthew Tancik, Ethan Weber, Evonne Ng, Ruilong Li, Brent Yi, Justin Kerr, Terrance Wang, Alexander Kristoffersen, Jake Austin, Kamyar Salahi, Abhik Ahuja, David McAllister, Angjoo Kanazawa.*<br> 
SIGGRAPH 2023. [[PDF](https://arxiv.org/abs/2302.04264)] [[Project](https://docs.nerf.studio/en/latest/)] [[Code](https://github.com/nerfstudio-project/nerfstudio/)]

**[A Survey on Deep Generative 3D-aware Image Synthesis.](https://arxiv.org/abs/2210.14267)**<br>
*Weihao Xia, Jing-Hao Xue.*<br>
ACM Computing Surveys 2023.

**[Differentiable Rendering: A Survey.](https://arxiv.org/abs/2006.12057)**<br>
*Hiroharu Kato, Deniz Beker, Mihai Morariu, Takahiro Ando, Toru Matsuoka, Wadim Kehl, Adrien Gaidon.*<br>

**[NeRF: Neural Radiance Field in 3D Vision, A Comprehensive Review.](https://arxiv.org/abs/2210.00379)**<br>
*Kyle Gao, Yina Gao, Hongjie He, Denning Lu, Linlin Xu, Jonathan Li.*<br>