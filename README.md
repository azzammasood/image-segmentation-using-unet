# Project: Image Segmentation using Unet

A U-Net is composed of an encoder and a decoder. The encoder convolves the input image, increasing channels and reducing spacial dimensions. The decoder deconvolves the image, reducing channels and increasing spatial dimensions. The tensor that is passed in the decoder is usually called bottleneck. At the end, the spatial dimensions are restored to make a prediction for each pixel in the input image. These types of models are extremely utilized in real world applications. 

Coded in Google Colab, this project features the U-Net which improves on the Fully Convolutional Network, using a somewhat similar design, but different in a few ways. Instead of one transposed convolution at the end of the network, it uses a matching number of convolutions for downsampling the input image to a feature map, and transposed convolutions for upsampling those maps back up to the original input image size. It also adds skip connections, to retain information that would otherwise become lost during encoding. Skip connections send information to every upsampling layer in the decoder from the corresponding downsampling layer in the encoder, capturing finer information while also keeping computation low. These help prevent information loss, as well as model overfitting. 

Phases:
  1. Implementing semantic image segmentation on the CARLA self-driving car dataset
  2. Applying sparse categorical crossentropy for pixelwise prediction
