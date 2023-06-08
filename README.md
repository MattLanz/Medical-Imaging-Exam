# Medical-Imaging-Exam
Project for Medical Imaging exam, involving the application of 3 Neural Networks for brain cancer segmentation from MR images

![resunet](https://github.com/MattLanzUnimib/Medical-Imaging-Exam/assets/98222024/7bda0091-dbd3-4445-b78b-26a0a1def9fc)

## Dataset
For this exam we decided to use The BRATS (Brain Tumor Segmentation) dataset, a widely used and highly valuable resource in the field of medical imaging and computer vision. It is specifically designed for the task of brain tumor segmentation and aims to advance the development and evaluation of algorithms for automated brain tumor detection and classification.
The BRATS dataset consists of 3D magnetic resonance imaging (MRI) scans of the brain, obtained from both glioma patients and healthy individuals. The dataset comprises multiple modalities, including T1-weighted, T1-weighted with contrast, T2-weighted, and fluid-attenuated inversion recovery (FLAIR) MRI sequences. Each MRI scan is accompanied by a corresponding ground truth label map that delineates different regions of the brain, such as the necrotic core, enhancing tumor, edema, and non-enhancing tumor.


## Models
In this project, we explored and implemented three popular architectures for brain tumor segmentation on the BRATS (Brain Tumor Segmentation) dataset. The models utilized were UNet, Residual UNet, and SegNet. Each of these models has demonstrated effectiveness in various medical imaging tasks and has been widely adopted by the research community.

### UNet
UNet is a convolutional neural network architecture commonly used for semantic segmentation tasks. It consists of an encoder-decoder structure with skip connections, allowing for the extraction of both low-level and high-level features. The encoder downsamples the input image, while the decoder upsamples the feature maps to generate segmentation masks. The skip connections help to retain spatial information and enable precise localization of object boundaries.

### Residual UNet
The Residual UNet is an extension of the UNet architecture that incorporates residual connections inspired by the ResNet model. Residual connections help alleviate the vanishing gradient problem and enable efficient information flow across the network. By combining the strengths of UNet and ResNet, the Residual UNet model enhances both feature extraction and localization capabilities.

### SegNet
SegNet is another popular architecture designed for semantic segmentation tasks, particularly suited for applications with limited computational resources. It comprises an encoder-decoder structure where the encoder performs downsampling operations, and the decoder performs upsampling. However, unlike UNet, SegNet employs pooling indices during the downsampling phase to preserve spatial information, which is crucial for precise segmentation.

## Model Comparison
Throughout our experiments, we thoroughly evaluated the performance of each model using the Dice coefficient. We conducted extensive training, validation, and testing to assess the models' generalization and robustness.

![Screenshot 2023-05-21 112215](https://github.com/MattLanzUnimib/Medical-Imaging-Exam/assets/98222024/ef96302b-cb03-40c8-92c4-80d6f2793ca8)

By employing UNet, Residual UNet, and SegNet on the BRATS dataset, we aimed to explore the strengths and limitations of each architecture for brain tumor segmentation. The models served as valuable tools in advancing our understanding of tumor characteristics and assisting in clinical decision-making.

Please refer to the model-specific documentation and source code for further details on the implementation, network architectures, and training configurations. 
