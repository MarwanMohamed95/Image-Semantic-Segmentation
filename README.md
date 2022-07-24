# **Image Semantic Segmentation**


![p](https://github.com/MarwanMohamed95/Image-Semantic-Segmentation/blob/main/UNet%20output.png?raw=true)

In this Project, we will do Image Semantic Segmentation using Fully Convolutional Network (FCN) and U-Net.

We will compare between the results of the two networks and evaluate each of them.

For FCN We will be using a pretrained VGG-16 network for the feature extraction path, then followed by an FCN-8 network for upsampling and generating the predictions. The output will be a label map (i.e. segmentation mask) with predictions for 3 classes.
For UNet This architecture is also a fully convolutional network and is similar to FCN. A key difference is the use of skip connections from the encoder to the decoder. The output will be a label map (i.e. segmentation mask) with predictions for 3 classes.

We will be training the model on the [Oxford Pets - IIT dataset](https://www.robots.ox.ac.uk/~vgg/data/pets/) dataset. This contains pet images, their classes, segmentation masks.

This dataset is already included in TensorFlow Datasets and we can download it. 
The segmentation masks are included in versions 3 and above.

Total num examples is 7349, training set is  3680, testing set is 3669

FCN Architecture:
![fcn](https://github.com/MarwanMohamed95/Image-Semantic-Segmentation/blob/main/FCN-8.png?raw=true)

UNet Architecture
![unet](https://github.com/MarwanMohamed95/Image-Semantic-Segmentation/blob/main/UNet.png?raw=true)


## Some output results
FCN-8 Result:
![fcn](https://github.com/MarwanMohamed95/Image-Semantic-Segmentation/blob/main/FCN_output.png?raw=true)

UNet Result:
![unet](https://github.com/MarwanMohamed95/Image-Semantic-Segmentation/blob/main/UNet%20output.png?raw=true)

### Models Accuracy and Loss Curves:

FCN-8:
![fcn](https://github.com/MarwanMohamed95/Image-Semantic-Segmentation/blob/main/plot_FCN.png?raw=true)


UNet:
![unet](https://github.com/MarwanMohamed95/Image-Semantic-Segmentation/blob/main/plot_UNet.png?raw=true)


## **At the End We can concolude that UNet has better results than FCN-8 due to Skip connections and we used more blocks in the UNet model**
