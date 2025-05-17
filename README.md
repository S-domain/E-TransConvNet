# E-TransConvNet: An Enhanced Transformer and Convolutional Network for Medical Image Segmentation from Ultrasound and CT Images

Medical image segmentation in ultrasound and CT images plays a crucial role in the prevention, diagnosis, and treatment of various diseases and cancers. Convolutional neural networks (CNNs) are computationally efficient for medical image segmentation but struggle to capture long-range dependencies, which are essential for global contextual understanding. Transformers address this limitation through self-attention mechanisms. However, architectures composed solely of transformer blocks impose prohibitive computational costs and compromise local spatial continuity. To overcome these challenges, we propose E-TransConvNet, a hybrid framework that integrates a CNN backbone with a single enhanced transformer block, effectively balancing computational efficiency, local continuity, and global contextual reasoning. The enhanced transformer block introduces two novel components: a Convolution Attention Block (CAB), which captures global context while simultaneously modeling local spatial relationships by integrating depth-wise convolutional operations into multi-head self-attention mechanisms, and a Progressive Feature Enhancement Feed-Forward Network (PFE-FFN), which further refines boundary delineation by selectively capturing features across various receptive fields to preserve fine-grained structural details. Extensive experiments are conducted on six public medical image segmentation datasets spanning two medical imaging modalities to validate the capacity and effectiveness of E-TransConvNet. Our model achieves superior segmentation accuracy and enhanced boundary delineation across all evaluated datasets. [(Paper link)](https://www.sciencedirect.com/science/article/abs/pii/S0957417425016434)

#  E-TransConvNet Architecture

![ARC](https://github.com/S-domain/E-TransConvNet/blob/695d5b634324f9a2eed9f22eb35a26191d786258/Figures/ARC.png)

# Enhanced Transformer Block
![ETB](https://github.com/S-domain/E-TransConvNet/blob/cdfb8a8e9b073026624cc10f338cc705f1d128e5/Figures/ETB.png)

# Segmentation Results on the Kidney US Dataset
![ETB](https://github.com/S-domain/E-TransConvNet/blob/eb811931c50e8a87f2db7b1297a432959df84a94/Figures/Kidney_US2.png)


# Requirements
Python>= 3.7, Pytorch >= 2.0, TensorFlow >= 2.9

# Experimental Setting
All experiments were conducted using an NVIDIA GeForce RTX 2080 Ti GPU

# CNN and Transformer-based Models for Medical Image Segmentation

| Date    | Model     |Title                                                                                                                                                      | Code |
| :---:   | :---:     | :---:                                                                                                                                                     | :---:|
| 2023  | DSEU-net    | DSEU-net: A novel deep supervision SEU-net for medical ultrasound image segmentation [(Paper)](https://doi.org/10.1016/j.eswa.2023.119939) | [Code](https://github.com/CGPxy/DSEU-net)|
| 2023 | NU-net    | Rethinking the unpretentious U-net for medical ultrasound image segmentation [(Paper)](https://doi.org/10.1016/j.patcog.2023.109728)      | [Code](https://github.com/CGPzy/NU-net)|
| 2023 | Chen et. al. | Asymmetric U-shaped network with hybrid attention mechanism for kidney ultrasound images segmentation [(Paper)](https://doi.org/10.1016/j.eswa.2022.118847) | [Code](https://github.com/CGPxy/Asymmetric-U-net-for-ultrasound-segmentation)|
| 2023 | RRCNet    | RRCNet: Refinement residual convolutional network for breast ultrasound images segmentation [(Paper)](https://doi.org/10.1016/j.engappai.2022.105601) | [Code](https://github.com/CGPxy/RRCNet)|
| 2024 | MSDANet   | MSDANet: A multi-scale dilation attention network for medical image segmentation [(Paper)](https://doi.org/10.1016/j.bspc.2023.105889)    | [Code](https://github.com/1999luan/MSDANet)|
| 2021 | TransUNet | TransUNet: Transformers Make Strong Encoders for Medical Image Segmentation [(Paper)](https://arxiv.org/abs/2102.04306)                   | [Code](https://github.com/Beckschen/TransUNet)|
| 2021 | MedT      | Medical Transformer: Gated Axial-Attention for Medical Image Segmentation   [(Paper)](https://link.springer.com/chapter/10.1007/978-3-030-87193-2_4)      | [Code](https://github.com/jeya-maria-jose/Medical-Transformer)|
| 2023 | BPAT-UNet | BPAT-UNet: Boundary preserving assembled transformer UNet for ultrasound thyroid nodule segmentation [(Paper)](https://doi.org/10.1016/j.cmpb.2023.107614) | [Code](https://github.com/ccjcv/BPAT-UNet)|
| 2023 | H2Former  | H2Former: An Efficient Hierarchical Hybrid Transformer for Medical Image Segmentation [(Paper)](https://ieeexplore.ieee.org/document/10093768)      | [Code](https://github.com/NKUhealong/H2Former)|
| 2023 | DAE-Former| DAE-Former: Dual Attention-Guided Efficient Transformer for Medical Image Segmentation [(Paper)](https://link.springer.com/chapter/10.1007/978-3-031-46005-0_8)      | [Code](https://github.com/mindflow-institue/DAEFormer)|
| 2023 | META-Unet | META-Unet: Multi-Scale Efficient Transformer Attention Unet for Fast and High-Accuracy Polyp Segmentation [(Paper)](https://ieeexplore.ieee.org/document/10179485)    | [Code](https://github.com/szuzzb/META-Unet)|
| 2023 | MAXFormer | MAXFormer: Enhanced transformer for medical image segmentation with multi-attention and multi-scale features fusion [(Paper)](https://doi.org/10.1016/j.knosys.2023.110987)  | [Code](https://github.com/zhiwei-liang/MAXFormer)|
| 2024 | MedSAM    | Segment anything in medical images [(Paper)](https://www.nature.com/articles/s41467-024-44824-z)      | [Code](https://github.com/bowang-lab/MedSAM)|


# Medical Image Segmentation Ultrasound and CT Datasets

| Year    | Dataset     | Tissue  Type                           | Link|
| :---:   | :---:     | :---:                                                          | :---:|
| 2020  | BUSI   | Breast | [Link](https://www.kaggle.com/datasets/sabahesaraki/breast-ultrasound-images-dataset) |  
| 2022  | Kidney US  | Kidney| [Link](http://rsingla.ca/kidneyUS/) |
| 2021 | TMUS  | Transverse musculoskeletal| [Link](https://doi.org/10.17632/3jykz7wz8d.1) |
| 2021  | TGUS | Thyroid gland | [Link](https://github.com/haifangong/TRFE-Net-for-thyroid-nodule-segmentation) |
| 2010  | 3D-IRCADb-1  | Liver | [Link](https://www.kaggle.com/datasets/sarahelqersh/3dircadb1) |
| 2021  | CHAOS | Liver | [Link](https://chaos.grand-challenge.org/) |



#   Contact
mecusbans@gmail.com

#   Acknowledgments
The authors thank the Chongqing University for their support.


# Cite this article
Atabansi CC, Nie J, Huang J, Feng Y, Liu H, Xie J, Zhou X. E-TransConvNet: An Enhanced Transformer and Convolutional Network for Medical Image Segmentation from Ultrasound and CT Images. Expert Systems with Applications. 2025 May 5:128022. 

