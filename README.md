# Project: Image Segmentation using Unet

U-Net improves on the Fully Convolutional Network, or FCN, using a somewhat similar design, but differing in some important ways.  Instead of one transposed convolution at the end of the network, it uses a matching number of convolutions for downsampling the input image to a feature map, and transposed convolutions for upsampling those maps back up to the original input image size. It also adds skip connections, to retain information that would otherwise become lost during encoding. Skip connections send information to every upsampling layer in the decoder from the corresponding downsampling layer in the encoder, capturing finer information while also keeping computation low. These help prevent information loss, as well as model overfitting. 

Phases:
  1. Implement semantic image segmentation on the CARLA self-driving car dataset
  2. Apply sparse categorical crossentropy for pixelwise prediction
