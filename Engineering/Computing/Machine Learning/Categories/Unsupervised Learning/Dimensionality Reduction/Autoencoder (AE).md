# Overview

> An autoencoder is **a type of artificial neural network used to learn efficient codings of unlabeled data** (unsupervised learning). An autoencoder learns two functions: an encoding function that transforms the input data, and a decoding function that recreates the input data from the encoded representation.
# Types of Autoencoders
| Type                                  | Description                                               | Use case                          |
| ------------------------------------- | --------------------------------------------------------- | --------------------------------- |
| **Basic Autoencoder**                 | Fully connected encoder–decoder                           | Dimensionality reduction          |
| **Convolutional Autoencoder (CAE)**   | Uses Conv layers                                          | Image denoising, feature learning |
| **Denoising Autoencoder (DAE)**       | Learns to reconstruct clean data from noisy inputs        | Noise removal                     |
| **Sparse Autoencoder**                | Adds sparsity regularization to latent vector             | Feature extraction                |
| **[[Variational Autoencoder (VAE)]]** | Learns probabilistic latent space (using mean & variance) | Generative modeling               |
| **Contractive Autoencoder**           | Penalizes sensitivity to input perturbations              | Robust feature learning           |
| **Sequence Autoencoder (LSTM-based)** | Encoder–decoder using RNNs                                | NLP, time-series compression      |
# Applications

- **Dimensionality reduction** (unsupervised alternative to PCA)
- **[[Anomaly Detection]]** (reconstruction error as anomaly score)
- **Image denoising**
- **Data compression**
- **Feature learning / pretraining**
- **Generative models** (VAE, etc.)
# Links
## Articles
- [Visualizing Autoencoders with Tensorflow.js](https://douglasduhaime.com/posts/visualizing-latent-spaces.html)
- [A Simple AutoEncoder and Latent Space Visualization with PyTorch | by Tingsong Ou | Medium](https://medium.com/@outerrencedl/a-simple-autoencoder-and-latent-space-visualization-with-pytorch-568e4cd2112a)
- [Introduction to autoencoders.](https://www.jeremyjordan.me/autoencoders/)
- [Autoencoder](https://www.krishnabhattarai.com/autoencoder)
- [Autoencoders - MATLAB & Simulink](https://www.mathworks.com/discovery/autoencoder.html)
- [DO - A Comprehensive Guide to the Intuition, Mathematics, and Implementation of Autoencoders - Part 1](https://www.danielobeng.com/posts/2023-05-10-autoencodersv2.html)
- [Building Autoencoders in Keras](https://blog.keras.io/building-autoencoders-in-keras.html?ref=jeremyjordan.me)
## Videos
- [Autoencoders | Deep Learning Animated - YouTube](https://www.youtube.com/watch?v=hZ4a4NgM3u0)
- [(5) Autoencoders Explained Easily - YouTube](https://www.youtube.com/watch?v=xwrzh4e8DLs)
- [Simple Explanation of AutoEncoders - YouTube](https://www.youtube.com/watch?v=3jmcHZq3A5s&t=440s)
- [Introduction To Autoencoders In Machine Learning. - YouTube](https://www.youtube.com/watch?v=NZ97-lFEUq8)
- [Autoencoders - simply explained - YouTube](https://www.youtube.com/watch?v=LHEj842yOF4)
- [How Convolutional Autoencoders Work—Visually Explained - YouTube](https://www.youtube.com/watch?v=95TnRUug7PQ)
- [Simple Explanation of AutoEncoders - YouTube](https://www.youtube.com/watch?v=3jmcHZq3A5s)
- [Autoencoders | Deep Learning Animated - YouTube](https://www.youtube.com/watch?v=hZ4a4NgM3u0&t=1s)
- [Encoder Decoder Network - Computerphile - YouTube](https://www.youtube.com/watch?v=1icvxbAoPWc)
- [Deep Learning Decall Fall 2017 Day 6: Autoencoders and Representation Learning - YouTube](https://www.youtube.com/watch?v=R3DNKE3zKFk)
## Papers
- [[2003.05991] Autoencoders](https://arxiv.org/abs/2003.05991)
- [[2201.03898] An Introduction to Autoencoders](https://arxiv.org/abs/2201.03898)
- [deeplearningbook.org/contents/autoencoders.html?](https://www.deeplearningbook.org/contents/autoencoders.html)
## Interactive
- [Introduction to Autoencoders](https://introduction-to-autoencoders.vercel.app/)
## Repositories
- [gr-b/autoencoder-latent-space-visualization: 2-dimensional visualization of the latent space learned by a deep autoencoder on MNIST](https://github.com/gr-b/autoencoder-latent-space-visualization)
