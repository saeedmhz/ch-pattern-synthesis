# Enhancing Mechanical Metamodels with a Generative Model-Based Augmented Training Dataset
This repository contains code + data to regenerate the results of the metamodeling section presented in  
[**Link to the paper**](https://arxiv.org/abs/2203.04183)  

In this work, we train a _feed-forward convolutional neural network_ on a dataset of _heterogeneous hyperelastic materials_ going through _equibiaxial extension_ to predict the stored strain energy in unseen materials. Material heterogeneity is based on **Cahn-Hilliard** patterns and all results are obtained through Finite Element Simulations using [**FEniCS**](https://fenicsproject.org/).

We also show the effect of augmenting the training set by synthetically generated patterns. We specifically used three different _Generative Adversarial Networks_ ([**StyleGAN2-ADA**](https://github.com/NVlabs/stylegan2-ada), [**WGAN-GP**](https://arxiv.org/abs/1704.00028), and [**WGAN-CP**](https://arxiv.org/abs/1701.07875)), and two random-based methods to generate **Cahn-Hilliard**-like patterns.

![Artboard 1](https://user-images.githubusercontent.com/54042195/155399467-73932dcd-3a15-45cf-aa1d-c895c52af122.png)

## This repository contains the following
* Datasets ([`data.7z`](data.7z)): Compressed versions of the datasets used in this work for metamodel training and testing
* Jupyter Notebook ([`metamodel.ipynb`](metamodel.ipynb)): PyTorch implementation of our metamodel in addition to a more detailed explanation on metamodel and generative model training and testing
