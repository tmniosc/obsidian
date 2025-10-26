# Overview

- **Convolutional Neural Networks (CNNs)** are a class of **Deep Learning models** designed to process **grid-like data**, such as **images (2D grids of pixels)** or **audio spectrograms (2D time–frequency maps)**.  
- They are especially powerful for **computer vision** tasks like classification, detection, and segmentation.

- A CNN automatically learns **spatial patterns** (edges, textures, shapes, objects) by applying **filters (kernels)** that slide over the input data.

 - Unlike traditional neural networks that treat every pixel independently, CNNs **exploit the spatial structure** of images — nearby pixels are often related.

-  In essence:
> **CNNs learn hierarchies of features — from edges → shapes → objects — directly from data.**
# Advantages of CNNs

✅ **Parameter sharing** — the same filter is applied across the image → fewer parameters than fully connected nets.  
✅ **[[Translation invariance|Translation invariance]]** — detects features regardless of their position.  
✅ **Automatic feature extraction** — no need for manual feature engineering.  
✅ **Scalable and efficient** for high-dimensional inputs like images.

# CNN Architectures
| Model                     | Year | Key Innovation                               |
| ------------------------- | ---- | -------------------------------------------- |
| **LeNet-5**               | 1998 | Early CNN for digit recognition              |
| **AlexNet**               | 2012 | Deep CNN with ReLU + GPU training            |
| **VGGNet**                | 2014 | Simplicity (3×3 filters, deep stack)         |
| **GoogLeNet (Inception)** | 2014 | Parallel convolutions (multi-scale)          |
| **ResNet**                | 2015 | Skip connections (solves vanishing gradient) |
| **EfficientNet**          | 2019 | Scalable CNN with optimal width/depth        |
# Links
## Papers
- [[1511.08458] An Introduction to Convolutional Neural Networks](https://arxiv.org/abs/1511.08458)
- [[2004.02806] A Survey of Convolutional Neural Networks: Analysis, Applications, and Prospects](https://arxiv.org/abs/2004.02806)
- [Understanding of a convolutional neural network | IEEE Conference Publication | IEEE Xplore](https://ieeexplore.ieee.org/document/8308186)
- [A review of convolutional neural networks in computer vision | Artificial Intelligence Review](https://link.springer.com/article/10.1007/s10462-024-10721-6)
- [[1803.02129] A Non-Technical Survey on Deep Convolutional Neural Network Architectures](https://arxiv.org/abs/1803.02129?utm_source=chatgpt.com)
- [Deep Learning: Basics and Convolutional Neural Networks (CNNs) | SpringerLink](https://link.springer.com/protocol/10.1007/978-1-0716-3195-9_3?utm_source=chatgpt.com)
- [kayhanCVPR20translationInvarianceCNN.pdf](https://jvgemert.github.io/pub/kayhanCVPR20translationInvarianceCNN.pdf?utm_source=chatgpt.com)
- [Going Deeper With Convolutions](https://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Szegedy_Going_Deeper_With_2015_CVPR_paper.pdf)
- [Convolutional neural networks: an overview and application in radiology | Insights into Imaging](https://link.springer.com/article/10.1007/s13244-018-0639-9)
- [content](https://research-repository.griffith.edu.au/server/api/core/bitstreams/b17b55ad-283a-4b00-9c07-8688d8690e1b/content)
## Lecture Notes
- [CS231n Deep Learning for Computer Vision](https://cs231n.github.io/convolutional-networks/)
- [convnet](https://www.cs.toronto.edu/~lczhang/360/lec/w04/convnet.html)
## Articles
- [How do Convolutional Neural Networks work?](https://brandonrohrer.com/how_convolutional_neural_networks_work.html)
## Videos
- [How Convolutional Neural Networks work - YouTube](https://www.youtube.com/watch?v=FmpDIaiMIeA)
- [Convolutional Neural Networks Explained (CNN Visualized) - YouTube](https://www.youtube.com/watch?v=pj9-rr1wDhM)
- [Convolutional Neural Networks from Scratch | In Depth - YouTube](https://www.youtube.com/watch?v=jDe5BAsT2-Y&t=1s)
- [CNN Receptive Field | Deep Learning Animated - YouTube](https://www.youtube.com/watch?v=ip2HYPC_T9Q)
- [Convolutional Neural Networks from Scratch | In Depth - YouTube](https://www.youtube.com/watch?v=jDe5BAsT2-Y)
- [Convolutional Neural Networks (Course 4 of the Deep Learning Specialization) - YouTube](https://www.youtube.com/playlist?list=PLkDaE6sCZn6Gl29AoE31iwdVwSG-KnDzF)
- [CNN: Convolutional Neural Networks Explained - Computerphile - YouTube](https://www.youtube.com/watch?v=py5byOOHZM8)
- [Why do Convolutional Neural Networks work so well? - YouTube](https://www.youtube.com/watch?v=8iIdWHjleIs)
- [Machine Learning For Medical Image Analysis - How It Works - YouTube](https://www.youtube.com/watch?v=VKnoyiNxflk&list=PLFPH5bHUlaU_6ydKuN2MQrhWL8s_gZj2b&index=11)
### Visualizations
- [Neural Network 3D Simulation - YouTube](https://www.youtube.com/watch?v=3JQ3hYko51Y)
- [Neural Networks 3D Simulation - YouTube](https://www.youtube.com/watch?v=hIYR6qMXujE)
- [Convolutional Neural Network (CNN) Visualization - YouTube](https://www.youtube.com/watch?v=enjnRVUoH9g)
## Interactive
- [TensorSpace.js](https://tensorspace.org/index.html)
- [poloclub/cnn-explainer: Learning Convolutional Neural Networks with Interactive Visualization.](https://github.com/poloclub/cnn-explainer)
- [An Interactive Node-Link Visualization of Convolutional Neural Networks](https://adamharley.com/nn_vis/)
- [Convolutional neural network visualizer - Project blog by Stefan Sietzen](https://portfolio.stefansietzen.at/posts/cnn-vis/)
### Mnist
- [Xavablog – Deep Learning of MNIST handwritten digits](https://xavier.robin.name/en/blog/2022/06/11/deep-learning-of-mnist-handwritten-digits)
- [MNIST Digit Playground](https://www.ccom.ucsd.edu/~cdeotte/programs/MNIST.html)
- [okdalto/VisualizeMNIST: This project is real-time visualization of a network recognizing digits from user's input.](https://github.com/okdalto/VisualizeMNIST)
- [MNIST Draw](https://mco-mnist-draw-rwpxka3zaa-ue.a.run.app/)
- [Interactive MNIST Application - λ∇](https://gradientof.me/projects/interactivemnist/)
- [Interactive MNIST Classifier — Kevin Liu](https://www.kevinliu.net/projects/mnist)
- [Explainable AI Demos](https://lrpserver.hhi.fraunhofer.de/handwriting-classification)
- [Interactive Mnist Classification](https://qianwen.info/demos/pset1/)
- [MNIST Image Classification - test online with Python and ConvNet. Valentyn Sichkar](https://valentynsichkar.name/mnist.html)
- [drewvlaz/draw-mnist: An interactive UI for MNIST using PyGame.](https://github.com/drewvlaz/draw-mnist)