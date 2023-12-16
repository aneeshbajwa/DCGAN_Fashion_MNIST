# DCGAN_Fashion_MNIST
Trained Deep Convolutional Generative Adversarial Netwrok (DCGAN) on tensorflow's Fashion MNIST dataset

Generator is an upsampling network with fractionally-strided convolutions

Discriminator is a convolutional network

Foolowed following architecture guidelines for stable Deep Convolutional GANs (source - https://arxiv.org/pdf/1511.06434.pdf):

Replace any pooling layers with strided convolutions (discriminator) and fractional-strided convolutions (generator).
Use batchnorm in both the generator and the discriminator.
Remove fully connected hidden layers for deeper architectures.
Use ReLU activation in generator for all layers expect for the output, which uses Tanh.
Use LeakyReLU activation in the discriminator for all layers.

