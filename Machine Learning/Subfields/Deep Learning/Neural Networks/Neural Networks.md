# Overview

A **Neural Network (NN)** is a computational model composed of interconnected processing units (**neurons**) that learn complex mappings from input to output data through **weighted connections** and **non-linear activations**.

It can learn representations across different data domains — from simple fixed-size vectors to structured or geometric data such as grids, sequences, and graphs.
# Architectures
| **Category**                      | **Architecture**                           | **Input Type**              | **Geometric Type**                     | **Examples / Applications**                  | **[[Inductive Bias]]**                                                                     |
| --------------------------------- | ------------------------------------------ | --------------------------- | -------------------------------------- | -------------------------------------------- | ------------------------------------------------------------------------------------------ |
| **Non-Geometric Neural Networks** | **Feedforward Neural Network (FNN / MLP)** | Fixed-size vector           | ❌ None (non-geometric)                 | Tabular data, regression, classification     | No structural bias; treats inputs independently                                            |
|                                   | **[[Recurrent Neural Network]] (RNN)**     | Sequential (1D)             | ⚪ 1D Euclidean (temporal / sequential) | Text, speech, time series                    | Sequential / temporal dependency; shared weights over time                                 |
| **[[Geometric Neural Networks]]** | **[[Convolution Neural Network]] (CNN)**   | Grid-like (2D/3D Euclidean) | ✅ Euclidean (spatial)                  | Image, video, computer vision                | Locality (neighboring pixels), translation equivariance, weight sharing                    |
|                                   | **[[Graph neural network]] (GNN)**         | Graph-structured data       | ✅ Non-Euclidean (relational / graph)   | Social networks, molecules, knowledge graphs | Relational / topological bias; permutation invariance; local aggregation (message passing) |
|                                   | **Point-based / Mesh / Manifold Networks** | Point clouds, 3D surfaces   | ✅ Non-Euclidean (geometric / manifold) | 3D vision, robotics, physical simulation     | Geometric / spatial bias; invariance to point ordering; local neighborhood aggregation     |
- [[Visualize Architecture of Neural Network]]
# Foundations of Neural Networks
- [[Universal Approximation Theorem]] (UAT)  
- [[Perceptron]]
- [[Gradient Descent]]
- [[Backpropagation]]
- [[Loss Landscape]]
## Links

### Books
- [Mathematical Engineering of Deep Learning](https://deeplearningmath.org/)
- [math-deep.pdf](https://www.cis.upenn.edu/~jean/math-deep.pdf)
### Papers
- [[1802.01528] The Matrix Calculus You Need For Deep Learning](https://arxiv.org/abs/1802.01528)
- [2203.08890](https://arxiv.org/pdf/2203.08890)
- [2310.20360](https://arxiv.org/pdf/2310.20360)
- [1802.01528](https://arxiv.org/pdf/1802.01528)
# Links

## Blogs
- [Home](https://www.krishnabhattarai.com/home)
## Books
-  [Neural networks and deep learning](http://neuralnetworksanddeeplearning.com/)
## Lecture Notes
- [APS360 Fundamentals of AI](https://www.cs.toronto.edu/~lczhang/360/lec/w04/lec06.pdf)
- [APS360 Artificial Intelligence Fundamentals (Summer 2019)](https://www.cs.toronto.edu/~lczhang/360/)
## Papers
- [NatureDeepReview.pdf](https://www.cs.toronto.edu/~hinton/absps/NatureDeepReview.pdf)
- [Deep learning](https://hal.science/hal-04206682/file/Lecun2015.pdf)
- [DeepLearning2July2014.pdf](https://people.idsia.ch/~juergen/DeepLearning2July2014.pdf)
## Articles
- [Looking inside neural nets](https://ml4a.github.io/ml4a/looking_inside_neural_nets/)
- [Neural Network](https://www.krishnabhattarai.com/neuralnetwork)
- [Experiments in Handwriting with a Neural Network](https://distill.pub/2016/handwriting/)
- [GRAIL Text Recognizer](https://jackschaedler.github.io/handwriting-recognition/)
## Videos
- [The Neural Network, A Visual Introduction - YouTube](https://www.youtube.com/watch?v=UOvPeC8WOt8&t=4s)
- [What happens *inside* a neural network? - YouTube](https://www.youtube.com/watch?v=-at7SLoVK_I)
- [What Are Neural Networks Even Doing? (Manifold Hypothesis) - YouTube](https://www.youtube.com/watch?v=pdNYw6qwuNc)
- [What Do Neural Networks Really Learn? Exploring the Brain of an AI Model - YouTube](https://www.youtube.com/watch?v=jGCvY4gNnA8)
- [How Neural Networks Learn Concepts - YouTube](https://www.youtube.com/watch?v=e5xKayCBOeU)
- [Dendrites: Why Biological Neurons Are Deep Neural Networks - YouTube](https://www.youtube.com/watch?v=hmtQPrH-gC4)
- [The Misconception that Almost Stopped AI [How Models Learn Part 1] - YouTube](https://www.youtube.com/watch?v=NrO20Jb-hy0)
- [Why Deep Learning Works Unreasonably Well [How Models Learn Part 3] - YouTube](https://www.youtube.com/watch?v=qx7hirqgfuU)
- [Building a neural network FROM SCRATCH (no Tensorflow/Pytorch, just numpy & math) - YouTube](https://www.youtube.com/watch?v=w8yWXqWQYmU)
- [I Built a Neural Network from Scratch - YouTube](https://www.youtube.com/watch?v=cAkMcPfY_Ns)
- [I Made an AI with just Redstone! - YouTube](https://www.youtube.com/watch?v=DQ0lCm0J3PM)
- [Deep Learning - Computerphile - YouTube](https://www.youtube.com/watch?v=TJlAxW-2nmI)
- [Inside a Neural Network - Computerphile - YouTube](https://www.youtube.com/watch?v=BFdMrDOx_CM)
- [How Deep Neural Networks Work - Full Course for Beginners - YouTube](https://www.youtube.com/watch?v=dPWYUELwIdM)
### Playlists
- [Neural networks - YouTube](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)
- [Neural Networks Demystified - YouTube](https://www.youtube.com/playlist?list=PLiaHhY2iBX9hdHaRr6b7XevZtgZRa1PoU)
## Interactive
- [A Neural Network Playground](https://playground.tensorflow.org/#activation=tanh&batchSize=10&dataset=circle&regDataset=reg-plane&learningRate=0.03&regularizationRate=0&noise=0&networkShape=4,2&seed=0.28131&showTestData=false&discretize=false&percTrainData=50&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false&hideText=false)
- [Neural Network Playground](https://www.ccom.ucsd.edu/~cdeotte/programs/neuralnetwork.html)
- [A Visual And Interactive Look at Basic Neural Network Math – Jay Alammar – Visualizing machine learning one concept at a time.](https://jalammar.github.io/feedforward-neural-networks-visual-interactive/)
- [Neural Network Playground - a Hugging Face Space by ameerazam08](https://huggingface.co/spaces/ameerazam08/neural-network-playground)
## Visualizations
- [Visualization of a fully connected neural network, version 1 - YouTube](https://www.youtube.com/watch?v=Tsvxx-GGlTg)
- [Visualization of a fully connected neural network, version 2 - YouTube](https://www.youtube.com/watch?v=sDDjJRnnHao)
- [neural network visualization 4k LQTWKCL 1 - YouTube](https://www.youtube.com/watch?v=UiQyMSKez7k)
- [VGG16 Neural Network Visualization - YouTube](https://www.youtube.com/watch?v=RNnKtNrsrmg)

