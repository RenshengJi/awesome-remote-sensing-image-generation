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


### 3. [NIPS '2024] ZoomLDM: Latent Diffusion Model for multi-scale image generation
**Authors**: Srikar Yellapragada, Alexandros Graikos, Kostas Triaridis, Prateek Prasanna, Rajarsi R. Gupta, Joel Saltz, Dimitris Samaras
<details span>
<summary><b>Abstract</b></summary>
  Diffusion models have revolutionized image generation, yet several challenges restrict their application to large-image domains, such as digital pathology and satellite imagery. Given that it is infeasible to directly train a model on 'whole' images from domains with potential gigapixel sizes, diffusion-based generative methods have focused on synthesizing small, fixed-size patches extracted from these images. However, generating small patches has limited applicability since patch-based models fail to capture the global structures and wider context of large images, which can be crucial for synthesizing (semantically) accurate samples. In this paper, to overcome this limitation, we present ZoomLDM, a diffusion model tailored for generating images across multiple scales. Central to our approach is a novel magnification-aware conditioning mechanism that utilizes self-supervised learning (SSL) embeddings and allows the diffusion model to synthesize images at different 'zoom' levels, i.e., fixed-size patches extracted from large images at varying scales. ZoomLDM achieves state-of-the-art image generation quality across all scales, excelling particularly in the data-scarce setting of generating thumbnails of entire large images. The multi-scale nature of ZoomLDM unlocks additional capabilities in large image generation, enabling computationally tractable and globally coherent image synthesis up to 4096×4096 pixels and 4× super-resolution. Additionally, multi-scale features extracted from ZoomLDM are highly effective in multiple instance learning experiments.
</details>

  [📄 Paper](https://arxiv.org/pdf/2411.16969v1) | 💻 Code | [🌐 Project Page](https://histodiffusion.github.io/docs/publications/zoomldm/)  


### 4. [CVPR '2024] Learned representation-guided diffusion models for large-image generation
**Authors**: Alexandros Graikos, Srikar Yellapragada, Minh-Quan Le, Saarthak Kapse, Prateek Prasanna, Joel Saltz, Dimitris Samaras
<details span>
<summary><b>Abstract</b></summary>
  To synthesize high-fidelity samples, diffusion models typically require auxiliary data to guide the generation process. However, it is impractical to procure the painstaking patch-level annotation effort required in specialized domains like histopathology and satellite imagery; it is often performed by domain experts and involves hundreds of millions of patches. Modern-day self-supervised learning (SSL) representations encode rich semantic and visual information. In this paper, we posit that such representations are expressive enough to act as proxies to fine-grained human labels. We introduce a novel approach that trains diffusion models conditioned on embeddings from SSL. Our diffusion models successfully project these features back to high-quality histopathology and remote sensing images. In addition, we construct larger images by assembling spatially consistent patches inferred from SSL embeddings, preserving long-range dependencies. Augmenting real data by generating variations of real images improves downstream classifier accuracy for patch-level and larger, image-scale classification tasks. Our models are effective even on datasets not encountered during training, demonstrating their robustness and generalizability. Generating images from learned embeddings is agnostic to the source of the embeddings. The SSL embeddings used to generate a large image can either be extracted from a reference image, or sampled from an auxiliary model conditioned on any related modality (e.g. class labels, text, genomic data). As proof of concept, we introduce the text-to-large image synthesis paradigm where we successfully synthesize large pathology and satellite images out of text descriptions.
</details>

  [📄 Paper](https://arxiv.org/pdf/2312.07330) | [💻 Code](https://github.com/cvlab-stonybrook/Large-Image-Diffusion) | [🌐 Project Page](https://histodiffusion.github.io/docs/publications/large_image)  
