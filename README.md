# DEFN: Dual-Encoder Fourier Group Harmonics Network for Three-Dimensional Macular Hole Reconstruction with Stochastic Retinal Defect Augmentation and Dynamic Weight Composition 

### [Project page](https://github.com/IIPL-HangzhouDianziUniversity/DEFN-Pytorch) | [Paper]()

DEFN: Dual-Encoder Fourier Group Harmonics Network for Three-Dimensional Macular Hole Reconstruction with Stochastic Retinal Defect Augmentation and Dynamic Weight Composition.<be>

Xingru Huang, Yihao Guo, Jian Huang, Zhi Li, Tianyun Zhang, Kunyan Cai, Gaopeng Huang, Wenhao Chen, Zhaoyang Xu, Liangqiong Qu, Ji Hu, Tinyu Wang, Shaowei Jiang, Chenggang Yan, Yaoqi Sun, Xin Ye, Yaqi Wang

Hangzhou Dianzi University

<div align=center>
  <img src="https://github.com/IIPL-HangzhouDianziUniversity/DEFN-Pytorch/blob/main/images/System_structure.png">
</div>
<p align=center>
  Figure 1: The System structure.
</p>

<div align=center>
  <img src="https://github.com/IIPL-HangzhouDianziUniversity/DEFN-Pytorch/blob/main/images/Network_structure.png">
</div>
<p align=center>
  Figure 2: The network structure of DEFN. 
</p>

We proposed DEFN, a 3D OCT segmentation network for eye diseases with unobvious characteristics and easy to be interfered with, such as macular hole and macular edema.

This repository contains the official Pytorch implementation for DEFN networking and DWC Loss, as well as the pre-trained model for DEFN.

## Methods
### FuGH Module

<div align=center>
  <img src="https://github.com/IIPL-HangzhouDianziUniversity/DEFN-Pytorch/blob/main/images/FuGH.png"width=50% height=50%>
</div>
<p align=center>
  Figure 3: The FuGH Module
</p>

The Fourier Group Harmonics (FuGH) module enhances noise reduction in OCT images by employing Fourier transformation for feature extraction in the frequency domain, enabling targeted noise filtration and efficient processing of periodic patterns with reduced computational complexity.

### S3DSA Module
<div align=center>
  <img src="https://github.com/IIPL-HangzhouDianziUniversity/DEFN-Pytorch/blob/main/images/S3DSA.png>
</div>
<p align=center>
  Figure 4: The S3DSA Module
</p>

The Simplified 3D Spatial Attention (S3DSA) module improves the segmentation of macular holes and edema in retinal images by optimizing spatial attention mechanisms.  It refines focus on crucial regions, enhancing segmentation quality and computational efficiency.

<div align=center>
  <img src="https://github.com/IIPL-HangzhouDianziUniversity/DEFN-Pytorch/blob/main/images/HSE.png>
</div>
<p align=center>
  Figure 5: The HSE Module
</p>

The Harmonic Squeeze-and-Excitation Module (HSE) combines Fourier Group Harmonics (FuGH) and Squeeze-and-Excitation (SE) blocks to enhance segmentation of macular holes and edema, by extending the model's view field and recalibrating feature weights.


