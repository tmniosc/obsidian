# [[Machine Learning]]

```
Machine Learning
│
├── 1️⃣ Supervised Learning
│     ├── Classification
│     │     ├── Binary / Multi-class / Multi-label
│     │     ├── CNN-based (ResNet, DenseNet, ViT)
│     │     ├── RNN/LSTM-based (Sequence Classification)
│     │     └── Transformer-based (BERT, RoBERTa)
│     │
│     ├── Regression
│     │     ├── Linear / Polynomial
│     │     ├── SVR (Support Vector Regression)
│     │     └── Neural Regression (MLP, Deep MLP)
│     │
│     └── Sequence Modeling
│           ├── RNN / LSTM / GRU
│           ├── Seq2Seq (Encoder–Decoder)
│           ├── Attention Mechanisms
│           └── Transformers (BERT, GPT, T5)
│
├── 2️⃣ Unsupervised Learning
│     ├── Clustering
│     │     ├── K-Means, DBSCAN, Hierarchical
│     │     ├── Spectral Clustering
│     │     └── Density-based / Graph-based clustering
│     │
│     ├── Dimensionality Reduction
│     │     ├── PCA, ICA, t-SNE, UMAP
│     │     └── Autoencoder (AE)
│     │
│     └── Generative Modeling
│           ├── Variational Autoencoder (VAE)
│           ├── Generative Adversarial Network (GAN)
│           ├── Flow-based Models (RealNVP, Glow)
│           └── Diffusion Models (DDPM, Stable Diffusion)
│
├── 3️⃣ Semi-Supervised Learning
│     ├── Pseudo-labeling
│     ├── Consistency Regularization (Mean Teacher, VAT)
│     ├── MixMatch / FixMatch
│     └── Semi-supervised Contrastive Learning (SimCLR-Semi)
│
├── 4️⃣ Reinforcement Learning
│     ├── Model-free
│     │     ├── Value-based (Q-Learning, DQN, DDQN)
│     │     └── Policy-based (REINFORCE, PPO, A3C, SAC)
│     │
│     ├── Model-based
│     │     ├── World Models, PlaNet, Dreamer
│     │     └── MuZero, MBPO
│     │
│     ├── Hierarchical RL
│     └── Meta-RL (RL², PEARL)
│
├── 5️⃣ Transfer Learning ⭐
│     │
│     ├── Feature-based Transfer
│     │     ├── Fine-tuning (ResNet, ViT, BERT)
│     │     ├── Feature Extraction (frozen backbone)
│     │     └── Linear Probing (evaluate embeddings)
│     │
│     ├── Domain Adaptation
│     │     ├── Unsupervised Domain Adaptation (UDA)
│     │     ├── Adversarial Domain Adaptation (DANN, ADDA)
│     │     ├── Domain Generalization (MetaDG)
│     │     └── Style Transfer (CycleGAN)
│     │
│     ├── Multi-task Learning
│     │     ├── Hard Parameter Sharing
│     │     └── Soft Sharing (task-specific heads)
│     │
│     ├── Cross-modal Transfer
│     │     ├── Vision ↔ Text (CLIP, ALIGN)
│     │     ├── Audio ↔ Video (AudioCLIP, VideoCLIP)
│     │     └── Vision ↔ Language ↔ Audio (ImageBind)
│     │
│     └── Foundation Model Fine-tuning
│           ├── Adapter Tuning / LoRA / Prefix Tuning
│           ├── Instruction Tuning / Alignment (RLHF, DPO)
│           ├── Visual Instruction Tuning (LLaVA, MiniGPT)
│           └── Domain-specific Fine-tuning (BioBERT, CodeBERT)
│
├── 6️⃣ Representation Learning
│     │
│     ├── Supervised Representation Learning
│     │     ├── Deep Feature Extraction (CNN, ViT)
│     │     ├── Metric Learning (Triplet / Contrastive Loss)
│     │     └── FaceNet, ArcFace
│     │
│     └── Self-Supervised Learning (SSL)
│           │
│           ├── 🔹 Contrastive Learning
│           │     ├── Instance-level
│           │     │     ├── SimCLR (Google, 2020)
│           │     │     ├── MoCo (v1, v2, v3)
│           │     │     ├── InfoNCE (core loss)
│           │     │     ├── CPC (Contrastive Predictive Coding)
│           │     │     └── PIRL (Pretext-Invariant Representation Learning)
│           │     │
│           │     ├── Momentum-based
│           │     │     ├── MoCo v1
│           │     │     ├── MoCo v2
│           │     │     ├── MoCo v3 (ViT backbone)
│           │     │     └── BYOL (Bootstrap Your Own Latent – no negatives)
│           │     │
│           │     └── Non-contrastive / Collapse-avoidance
│           │           ├── SimSiam
│           │           ├── Barlow Twins
│           │           ├── VICReg / VICRegL
│           │           ├── DINO / DINOv2
│           │           ├── EsViT
│           │           └── ReLIC / ReLICv2
│           │
│           ├── 🔹 Predictive / Pretext Tasks
│           │     ├── Context Prediction
│           │     ├── Jigsaw Puzzles
│           │     ├── Rotation Prediction (RotNet)
│           │     ├── Colorization
│           │     ├── Inpainting (Image Completion)
│           │     ├── Masked Prediction (MAE, BEiT)
│           │     └── Temporal Order Prediction (Video)
│           │
│           ├── 🔹 Generative SSL
│           │     ├── Autoencoder / VAE
│           │     ├── Masked Autoencoder (MAE, BEiT, iBOT)
│           │     └── GAN-based SSL (BiGAN, ALI)
│           │
│           ├── 🔹 Self-Distillation & Knowledge Distillation
│           │     ├── BYOL / SimSiam
│           │     ├── DINO / DINOv2
│           │     ├── EsViT / DeiT
│           │     ├── BEiTv2 / iBOT
│           │     └── Noisy Student Training
│           │
│           └── 🔹 Multimodal Self-Supervised Learning
│                 ├── CLIP (Text–Image contrastive, OpenAI)
│                 ├── ALIGN (Google)
│                 ├── FLAVA (Meta AI)
│                 ├── BLIP / BLIP-2 (Salesforce)
│                 ├── AudioCLIP / VideoCLIP
│                 ├── UniVL (Video-Language)
│                 ├── ImageBind (Meta, 2023)
│                 └── Kosmos-2 / GPT-4V (Vision-Language)
│
├── 7️⃣ Few-shot / Meta Learning
│     ├── Metric-based
│     │     ├── Siamese Network
│     │     ├── Triplet Network
│     │     ├── Prototypical Network
│     │     └── Matching Network
│     │
│     ├── Optimization-based
│     │     ├── MAML (Model-Agnostic Meta Learning)
│     │     ├── Reptile
│     │     └── ANIL
│     │
│     └── Memory-based
│           ├── Neural Turing Machine (NTM)
│           └── Memory-Augmented Neural Network (MANN)
│
└── 8️⃣ Foundation & Multimodal Models
      ├── Vision–Language (CLIP, BLIP, Kosmos, Flamingo)
      ├── Large Language Models (GPT, Gemini, LLaMA)
      ├── Multimodal Unified Models (ImageBind, VideoCLIP)
      ├── Diffusion-based Generative Models (Stable Diffusion, SDXL)
      └── Agentic AI (AutoGPT, Voyager, ReAct)
```

# [[Mathematics]]
```
MATHEMATICS
│
├── PURE MATHEMATICS
│   ├── 1. Foundations
│   │   ├── Mathematical Logic
│   │   ├── Set Theory
│   │   └── Category Theory
│   │
│   ├── 2. Algebra
│   │   ├── Linear Algebra
│   │   ├── Abstract Algebra (Groups, Rings, Fields)
│   │   ├── Commutative Algebra
│   │   └── Number Theory
│   │
│   ├── 3. Analysis
│   │   ├── Real Analysis
│   │   ├── Complex Analysis
│   │   ├── Functional Analysis
│   │   └── Measure Theory
│   │
│   ├── 4. Geometry & Topology
│   │   ├── Euclidean & Non-Euclidean Geometry
│   │   ├── Algebraic Geometry
│   │   ├── Differential Geometry
│   │   ├── General Topology
│   │   └── Algebraic Topology
│   │
│   └── 5. DISCRETE MATHEMATICS                     ← **HERE (PURE)**
│       ├── Mathematical Logic
│       ├── Combinatorics
│       ├── Graph Theory
│       ├── Discrete Structures (Relations, Posets, Boolean Algebra)
│       └── Computational Number Theory
│           ↓↓↓ (Applications → see below)
│
└── APPLIED MATHEMATICS
    ├── 1. Mathematical Physics
    │   ├── Classical Mechanics
    │   ├── Quantum Mechanics
    │   └── Statistical Mechanics
    │
    ├── 2. PDEs & Numerical Analysis
    │   ├── ODEs / PDEs
    │   ├── Finite Element / Finite Difference Methods
    │   └── Monte Carlo & Computational Modeling
    │
    ├── 3. Probability & Statistics
    │   ├── Stochastic Processes
    │   ├── Statistical Inference
    │   └── Data Analysis & Machine Learning Foundations
    │
    ├── 4. Optimization & Control
    │   ├── Linear / Nonlinear Programming
    │   ├── Control Theory (LQR, PID)
    │   └── Game Theory
    │
    ├── 5. Financial & Actuarial Mathematics
    │   ├── Stochastic Calculus
    │   ├── Option Pricing (Black-Scholes)
    │   └── Risk Modeling
    │
    ├── 6. Mathematical Biology & Medicine
    │   ├── Population Dynamics (Lotka-Volterra)
    │   ├── Epidemiology (SIR/SEIR)
    │   └── Medical Imaging & Bioinformatics
    │
    ├── 7. Engineering & Signal Processing
    │   ├── Fourier / Wavelet Analysis
    │   ├── Image Processing
    │   └── Cryptography
    │
    └── 8. APPLICATIONS OF DISCRETE MATHEMATICS
        ├── Algorithms & Data Structures
        ├── Coding Theory & Error Correction
        ├── Network Optimization & Routing
        ├── Artificial Intelligence (Search, SAT, CSP)
        └── Cybersecurity (RSA, Hash Functions)
```


# Notes
`fnscio`
`cincoutvn`
`tmniosc`
