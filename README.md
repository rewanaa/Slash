# Overview
This project aims to classify images of clothes and bags using various deep learning models. The dataset used for this project is collected from the Slash application,
and it is available on [Kaggle](https://www.kaggle.com/datasets/comvisionnn/slash-dataset). The project involves preprocessing the data, augmenting the dataset due to its small size, building custom models like MobileNet and AlexNet from scratch,
and fine-tuning the pre-trained MobileNet model.

# [vedio](https://drive.google.com/drive/folders/1382nmjfKjOAwbnsyGjGLCuASsBFZv_um?usp=sharing)

# Dataset
The dataset consists of images of clothes and bags collected from the Slash application. It contains images of various types of clothing items and bags.
You can download the dataset from [Kaggle](https://www.kaggle.com/datasets/comvisionnn/slash-dataset).

# Preprocessing and Augmentation
-The dataset is split into training and testing sets with an 80-20 ratio.

-Image preprocessing involves resizing images to 256x256 pixels.

-Data augmentation techniques such as random horizontal flip, random rotation, color jitter, random erasing, and RandAugment are applied to increase the diversity of the dataset and improve model generalization.

# Models Architecture
## MobileNet from Scratch
A custom MobileNet model is implemented from scratch. It consists of depthwise separable convolutions and achieves lightweight and efficient feature extraction.

## AlexNet from Scratch
A custom AlexNet model is implemented from scratch. It follows the classic architecture of AlexNet with convolutional and fully connected layers.

## Fine-tuning Pre-trained MobileNet
A pre-trained MobileNet model is fine-tuned for the clothing and bag classification task. The final fully connected layer is modified, and the model is trained on the dataset.

# Results
#### The evaluation results for each model are as follows:

## Fine-tuned MobileNet
Accuracy: 100%

Inference Time: 0.05988

The fine-tuned MobileNet model achieved a perfect accuracy of 100% on the test dataset. This high accuracy is expected as the model was pre-trained on a large dataset and fine-tuned on the specific clothing and bag classification task.

## MobileNet (From Scratch)
Accuracy: 85%

Inference Time: 0.04141

The custom MobileNet model achieved an accuracy of 85% on the test dataset. Despite being trained from scratch, the model performed reasonably well, demonstrating its effectiveness in feature extraction and classification.

## AlexNet (From Scratch)
Accuracy: 76%

Inference Time: 0.03673

The custom AlexNet model achieved an accuracy of 76% on the test dataset. Although it performed slightly lower compared to MobileNet, it still demonstrated decent performance in classifying clothing and bags.

#### These results suggest that fine-tuning a pre-trained model like MobileNet can lead to superior performance compared to training models from scratch, especially when dealing with limited training data.

