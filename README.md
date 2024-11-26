# awesome-remote-sensing-image-generation

A curated list of papers and open-source resources focused on remote sensing image generation. 

### 1. [ICLR '2024] DiffusionSat: A Generative Foundation Model for Satellite Imagery
**Authors**: Samar Khanna, Patrick Liu, Linqi Zhou, Chenlin Meng, Robin Rombach, Marshall Burke, David Lobell, Stefano Ermon
<details span>
<summary><b>Abstract</b></summary>
  Diffusion models have achieved state-of-the-art results on many modalities including images, speech, and video. However, existing models are not tailored to support remote sensing data, which is widely used in important applications including environmental monitoring and crop-yield prediction. Satellite images are significantly different from natural images -- they can be multi-spectral, irregularly sampled across time -- and existing diffusion models trained on images from the Web do not support them. Furthermore, remote sensing data is inherently spatio-temporal, requiring conditional generation tasks not supported by traditional methods based on captions or images. In this paper, we present DiffusionSat, to date the largest generative foundation model trained on a collection of publicly available large, high-resolution remote sensing datasets. As text-based captions are sparsely available for satellite images, we incorporate the associated metadata such as geolocation as conditioning information. Our method produces realistic samples and can be used to solve multiple generative tasks including temporal generation, superresolution given multi-spectral inputs and in-painting. Our method outperforms previous state-of-the-art methods for satellite image generation and is the first large-scale generative foundation model for satellite imagery.
</details>

  [📄 Paper](https://arxiv.org/pdf/2312.03606) | [💻 Code](https://github.com/samar-khanna/DiffusionSat) | [🌐 Project Page](https://www.samarkhanna.com/DiffusionSat/)  


### 2. [Arxiv '2024] MetaEarth: A Generative Foundation Model for Global-Scale Remote Sensing Image Generation
**Authors**: Zhiping Yu, Chenyang Liu, Liqin Liu, Zhenwei Shi, Zhengxia Zou
<details span>
<summary><b>Abstract</b></summary>
  The recent advancement of generative foundational models has ushered in a new era of image generation in the realm of natural images, revolutionizing art design, entertainment, environment simulation, and beyond. Despite producing high-quality samples, existing methods are constrained to generating images of scenes at a limited scale. In this paper, we present MetaEarth, a generative foundation model that breaks the barrier by scaling image generation to a global level, exploring the creation of worldwide, multi-resolution, unbounded, and virtually limitless remote sensing images. In MetaEarth, we propose a resolution-guided self-cascading generative framework, which enables the generating of images at any region with a wide range of geographical resolutions. To achieve unbounded and arbitrary-sized image generation, we design a novel noise sampling strategy for denoising diffusion models by analyzing the generation conditions and initial noise. To train MetaEarth, we construct a large dataset comprising multi-resolution optical remote sensing images with geographical information. Experiments have demonstrated the powerful capabilities of our method in generating global-scale images. Additionally, the MetaEarth serves as a data engine that can provide high-quality and rich training data for downstream tasks. Our model opens up new possibilities for constructing generative world models by simulating Earth visuals from an innovative overhead perspective.
</details>

  [📄 Paper](https://arxiv.org/pdf/2405.13570) | [💻 Code](https://github.com/samar-khanna/DiffusionSat) | [🌐 Project Page](https://jiupinjia.github.io/metaearth/)  
