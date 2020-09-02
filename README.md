# GANs-Objective-implementation-application
This repo aims at understanding GAN, provides a small derivation of Generator and Discriminator objective functions and demonstrates application of GAN in pathology images and Context encoders (inpainting)


# Deep Convolution Generative Adversarial Networks

This example implements the paper [Unsupervised Representation Learning with Deep Convolutional Generative Adversarial Networks](http://arxiv.org/abs/1511.06434)


## Usage
```
usage: main.py [-h] --dataset DATASET --dataroot DATAROOT [--workers WORKERS]
               [--batchSize BATCHSIZE] [--imageSize IMAGESIZE] [--nz NZ]
               [--ngf NGF] [--ndf NDF] [--niter NITER] [--lr LR]
               [--beta1 BETA1] [--cuda] [--ngpu NGPU] [--netG NETG]
               [--netD NETD]

optional arguments:
  -h, --help            show this help message and exit
  --dataset DATASET     cifar10 | lsun | mnist |imagenet | folder | lfw | fake
  --dataroot DATAROOT   path to dataset
  --workers WORKERS     number of data loading workers
  --batchSize BATCHSIZE input batch size
  --imageSize IMAGESIZE the height / width of the input image to network
  --nz NZ               size of the latent z vector
  --ngf NGF
  --ndf NDF
  --niter NITER         number of epochs to train for
  --lr LR               learning rate, default=0.0002
  --beta1 BETA1         beta1 for adam. default=0.5
  --cuda                enables cuda
  --ngpu NGPU           number of GPUs to use
  --netG NETG           path to netG (to continue training)
  --netD NETD           path to netD (to continue training)
  --outf OUTF           folder to output images and model checkpoints
  --manualSeed SEED     manual seed
  --classes CLASSES     comma separated list of classes for the lsun data set
```
