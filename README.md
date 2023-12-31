## 1. Network Structure

* StyleGan系列：
1. A Style-Based Generator Architecture for Generative Adversarial Networks 
	* [NVlabs/stylegan: StyleGAN - Official TensorFlow Implementation (github.com)](https://github.com/NVlabs/stylegan)
2. Analyzing and Improving the Image Quality of StyleGAN   
	* [NVlabs/stylegan2: StyleGAN2 - Official TensorFlow Implementation (github.com)](https://github.com/NVlabs/stylegan2)

## 2. Avatar
### 2.1. Face
* A Morphable Model For The Synthesis Of 3D Faces 
	* https://github.com/MichaelMure/3DMM

* FLAME: Learning a model of facial shape and expression from 4D scans
	* [FLAME (mpg.de)](https://flame.is.tue.mpg.de/)

## 3. 3D Generation


* DreamFusion
	* [DreamFusion: Text-to-3D using 2D Diffusion (dreamfusion3d.github.io)](https://dreamfusion3d.github.io/)
	* Description：propose SDS loss

* ProlificDreamer
	* [ProlificDreamer: High-Fidelity and Diverse Text-to-3D Generation with Variational Score Distillation (tsinghua.edu.cn)](https://ml.cs.tsinghua.edu.cn/prolificdreamer/)
	* Description：propose VDS loss


* Magic3d
	* [Magic3D: High-Resolution Text-to-3D Content Creation (nvidia.com)](https://research.nvidia.com/labs/dir/magic3d/)
	* 两阶段生成，coarse-to-fine


* Magic123
	* [Magic123: One Image to High-Quality 3D Object Generation Using Both 2D and 3D Diffusion Priors (guochengqian.github.io)](https://guochengqian.github.io/project/magic123/)


* DreamCraft3D
	* [DreamCraft3D: Hierarchical 3D Generation with Bootstrapped Diffusion Prior (mrtornado24.github.io)](https://mrtornado24.github.io/DreamCraft3D/)

* DreamGaussian: Generative Gaussian Splatting for Efficient 3D Content Creation
	* [DreamGaussian](https://dreamgaussian.github.io/)



### 3D大模型

* zero-123
	* provide objaverse dataset [Objaverse (allenai.org)](https://objaverse.allenai.org/)
	* train a novel-view generator

* zero-123++


* One-2-3-45
	* [One-2-3-45](https://one-2-3-45.github.io/)
	* Use Zero123 to generate multi-view images for the input view, and then aim to lift them up to 3D space

* LRM: Large Reconstruction Model for Single Image to 3D
	* https://scalei3d.github.io/LRM/

* Instant3D: Fast Text-to-3D with Sparse-view Generation and Large Reconstruction Model
	* https://instant-3d.github.io

* DMV3D: Denoising Multi-view Diffusion Using 3D Large Reconstruction Model
	* https://dmv3d.github.io

* PF-LRM: Pose-Free Large Reconstruction Model for Joint Pose and Shape Prediction
	* https://totoro97.github.io/pf-lrm





## 4. 3D-Representation


* Indoor Segmentation and Support Inference from RGBD Images
	* 相当早期的标注深度数据集
	* 提出深度和normal预测方法
	* ECCV-12

* GeoNet
	* [xjqi/GeoNet: GeoNet: Geometric Neural Network for Joint Depth and Surface Normal Estimation (github.com)](https://github.com/xjqi/GeoNet)
	* CVPR 2018

* NeuS: Learning Neural Implicit Surfaces by Volume Rendering for Multi-view Reconstruction
	* [NeuS: Learning Neural Implicit Surfaces by Volume Rendering for Multi-view Reconstruction (lingjie0206.github.io)](https://lingjie0206.github.io/papers/NeuS/)
	* NeurIPS 2021 (Spotlight)
	* signed distance function (SDF) 与 neural SDF 表示

* 3D Gaussian Splatting for Real-Time Radiance Field Rendering
	* [3D Gaussian Splatting for Real-Time Radiance Field Rendering (inria.fr)](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/)
	* TOG 2023
	* 提供了一种整体思想类似Nerf但是效率更高的高斯点云方法


## To be done

MVDream: Multi-view Diffusion for 3D Generation
https://mv-dream.github.io/


adobe灌了四篇：

LRM: Large Reconstruction Model for Single Image to 3D
https://scalei3d.github.io/LRM/

Instant3D: Fast Text-to-3D with Sparse-view Generation and Large Reconstruction Model
https://instant-3d.github.io


DMV3D: Denoising Multi-view Diffusion Using 3D Large Reconstruction Model
https://dmv3d.github.io

PF-LRM: Pose-Free Large Reconstruction Model for Joint Pose and Shape Prediction
https://totoro97.github.io/pf-lrm


SweetDreamer: Aligning Geometric Priors in 2D diffusion for Consistent Text-to-3D

DMTet
[Deep Marching Tetrahedra: a Hybrid Representation for High-Resolution 3D Shape Synthesis (nvidia.com)](https://research.nvidia.com/labs/toronto-ai/DMTet/)

EG3D
[EG3D: Efficient Geometry-aware 3D GANs (nvlabs.github.io)](https://nvlabs.github.io/eg3d/)

[One-2-3-45++ (sudo-ai-3d.github.io)](https://sudo-ai-3d.github.io/One2345plus_page/)

[Instant Neural Graphics Primitives with a Multiresolution Hash Encoding (nvlabs.github.io)](https://nvlabs.github.io/instant-ngp/)
instant-ngp


[justimyhxu/awesome-3D-generation: A curated list of awesome 3d generation papers (github.com)](https://github.com/justimyhxu/awesome-3D-generation)

