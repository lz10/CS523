## CS523
# An application of CVAE on MINIST dataset
author: Linan Zhang, Jintian Cai

email: {lz1018,jtcai}@bu.edu

This project focuses on the Conditional Variantional Auto-encoder, a member of VAE family that is enabled to sampling new data conditional on a specific input.
- Traditional VAE model generates plausible looking fake samples while it could not control the model output. 
- The goal of this project aims to build up an auto-encoder model that could generate specific output.

## Conditional Variational Auto-encoder (CVAE)
In a one-sentence description, CVAE proceeds as conditioning the entire generative process on an input with the loss function as a sumation of KL divergence and cross-entropy loss.
- Dependencies
  - pytorch
  - matlabplotlib
  - keras
- Model arichitecture
![avatar](https://github.com/lz10/CS523/blob/main/picture/architecture%201.png)
![avatar](https://github.com/lz10/CS523/blob/main/picture/architecture%202.png)

- Experimental Setup
  - dataset: MNIST dataset in torchvision.datasets
  - Batchsize: 100
  - Activation function: Relu(x)
  - Optimizer: Adam
  - Epochs = 50
- Training and testing:
![avatar](https://github.com/lz10/CS523/blob/main/picture/training%20set.png)
![avatar](https://github.com/lz10/CS523/blob/main/picture/test%20set.png)

- Demos:
![avatar](https://github.com/lz10/CS523/blob/main/picture/demo.png)

## Full presentation slides
https://github.com/lz10/CS523/blob/main/Conditional%20VAE.pdf

## References
[1] Kihyuk Sohn, Honglak Lee, and Xinchen Yan. ‘Learning structured output representation using deep conditional generative models.’  _In NIPS_, 2015.

[2] Carl Doersch, ‘Tutorial on Variational Autoencoders’, _arXiv:1606.05908_, 2016

[3] Deng, L., 'The mnist database of handwritten digit images for machine learning research.' _IEEE Signal Processing Magazine_, 29(6), 141–142, 2012.

[4] https://github.com/lyeoni/pytorch-mnist-CVAE

[5] https://github.com/lyeoni/pytorch-mnist-VAE


