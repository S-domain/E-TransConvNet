# E-TransConvNet: An Enhanced Transformer and Convolutional Network for Medical Image Segmentation from Ultrasound and CT Images

Medical image segmentation in ultrasound and CT images plays a crucial role in the prevention, diagnosis, and treatment of various diseases and cancers. Convolutional neural networks (CNNs) are computationally efficient for medical image segmentation but struggle to capture long-range dependencies, which are essential for global contextual understanding. Transformers address this limitation through self-attention mechanisms. However, architectures composed solely of transformer blocks impose prohibitive computational costs and compromise local spatial continuity. To overcome these challenges, we propose E-TransConvNet, a hybrid framework that integrates a CNN backbone with a single enhanced transformer block, effectively balancing computational efficiency, local continuity, and global contextual reasoning. The enhanced transformer block introduces two novel components: a Convolution Attention Block (CAB), which captures global context while simultaneously modeling local spatial relationships by integrating depth-wise convolutional operations into multi-head self-attention mechanisms, and a Progressive Feature Enhancement Feed-Forward Network (PFE-FFN), which further refines boundary delineation by selectively capturing features across various receptive fields to preserve fine-grained structural details. Extensive experiments are conducted on six public medical image segmentation datasets spanning two medical imaging modalities to validate the capacity and effectiveness of E-TransConvNet. Our model achieves superior segmentation accuracy and enhanced boundary delineation across all evaluated datasets. [(Paper link)](https://www.sciencedirect.com/science/article/abs/pii/S0957417425016434)

#  E-TransConvNet Architecture

![ARC](https://github.com/S-domain/E-TransConvNet/blob/695d5b634324f9a2eed9f22eb35a26191d786258/Figures/ARC.png)

# Enhanced Transformer Block
![ETB](https://github.com/S-domain/E-TransConvNet/blob/cdfb8a8e9b073026624cc10f338cc705f1d128e5/Figures/ETB.png)

# Segmentation Results on the Kidney US Dataset
![ETB](https://github.com/S-domain/E-TransConvNet/blob/eb811931c50e8a87f2db7b1297a432959df84a94/Figures/Kidney_US2.png)

# License
This codes are released under the MIT License (refer to the LICENSE file for details).

# Requirements
Pytorch >= 2.0, TensorFlow >= 2.0

# CNN and Transformer-based Models for Medical Image Segmentation

| Date    | Model     |Title                                                                                                                                                      | Code |
| :---:   | :---:     | :---:                                                                                                                                                     | :---:|
| 2023  | DSEU-net    | DSEU-net: A novel deep supervision SEU-net for medical ultrasound image segmentation [(Paper)](https://doi.org/10.1016/j.eswa.2023.119939) | [Code](https://github.com/CGPxy/DSEU-net)|
| 2023 | NU-net    | Rethinking the unpretentious U-net for medical ultrasound image segmentation [(Paper)](https://doi.org/10.1016/j.patcog.2023.109728)      | [Code](https://github.com/CGPzy/NU-net)|


# Medical Image Ultrasound and CT Datasets

| Year    | Dataset     | Tissue  Type                           | Link|
| :---:   | :---:     | :---:                                                          | :---:|
| 2020  | BUSI   | Breast | [Link](https://www.kaggle.com/datasets/sabahesaraki/breast-ultrasound-images-dataset) |  
| 2022  | Kidney US  | Kidney| [Link](http://rsingla.ca/kidneyUS/) |
| 2021 | TMUS  | Transverse musculoskelet| [Link](https://doi.org/10.17632/3jykz7wz8d.1) |
| 2021  | TGUS | Thyroid gland | [Link](https://github.com/haifangong/TRFE-Net-for-thyroid-nodule-segmentation) |
| 2010  | 3D-IRCADb-1  | Liver | [Link](https://www.kaggle.com/datasets/sarahelqersh/3dircadb1) |
| 2021  | CHAOS | Liver | [Link](https://chaos.grand-challenge.org/) |



#   Contact
mecusbans@gmail.com

#   Acknowledgments
The authors thank the Chongqing University for their support.


# Cite this article
Atabansi CC, Nie J, Huang J, Feng Y, Liu H, Xie J, Zhou X. E-TransConvNet: An Enhanced Transformer and Convolutional Network for Medical Image Segmentation from Ultrasound and CT Images. Expert Systems with Applications. 2025 May 5:128022. 

