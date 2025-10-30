# Overview
**Machine Learning (ML)** is a field of **Artificial Intelligence (AI)** that focuses on building systems that can **learn from data** instead of being explicitly programmed.  
In short:

> “ML = Systems that learn from experience (data) to improve performance on a task.”

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

## Concepts
- [[Mathematical Foundations]]
- [[Inductive Bias]]
- [[No free lunch theorem]]
- [[Curse of Dimensionality]]
- [[Feature Extraction]]
- [[Data Augmentation]]
# Subfields
- [[Deep Learning]]
# Related fields
- [[Data Science]]
# Categories
- [[Supervised Learning]]
- [[Self-Supervised Learning]] 
- [[Unsupervised Learning]]
- [[Semi-Supervised Learning]]
- [[Reinforcement Learning]]
- [[Transfer Learning]]
- [[Representation Learning]]
- [[Few-shot - Meta Learning]]
- [[Foundation & Multimodal Models]]
# Links

## Articles
- [How to Learn Machine Learning in 2025 | DataCamp](https://www.datacamp.com/blog/how-to-learn-machine-learning)
- [How to Learn AI From Scratch in 2024: A Complete Expert Guide | DataCamp](https://www.datacamp.com/blog/how-to-learn-ai)
- [AI Expert Roadmap](https://i.am.ai/roadmap/#note)
- [Machine Learning is Fun!. The world’s easiest introduction to… | by Adam Geitgey | Medium](https://medium.com/@ageitgey/machine-learning-is-fun-80ea3ec3c471)
- [Do Machine Learning Models Memorize or Generalize?](https://pair.withgoogle.com/explorables/grokking/)
- [Can AI Solve Science?—Stephen Wolfram Writings](https://writings.stephenwolfram.com/2024/03/can-ai-solve-science/)
- [What Is ChatGPT Doing … and Why Does It Work?—Stephen Wolfram Writings](https://writings.stephenwolfram.com/2023/02/what-is-chatgpt-doing-and-why-does-it-work/)
## Tutorials
- [Machine Learning  |  Google for Developers](https://developers.google.com/machine-learning/)
- [Machine Learning for Artists](https://ml4a.github.io/ml4a/)
- [Machine Learning Glossary — ML Glossary documentation](https://ml-cheatsheet.readthedocs.io/en/latest/)
## Books
- [ML Systems Textbook](https://www.mlsysbook.ai/)
- [Interpretable Machine Learning](https://christophm.github.io/interpretable-ml-book/)
- [Hands-On-Machine-Learning/Hands-On Machine Learning with Scikit-Lear - Aurelien Geron.pdf at master · augaonkar/Hands-On-Machine-Learning](https://github.com/augaonkar/Hands-On-Machine-Learning/blob/master/Hands-On%20Machine%20Learning%20with%20Scikit-Lear%20-%20Aurelien%20Geron.pdf)
- [Machine Learning cơ bản](https://machinelearningcoban.com/)
- [tiepvupsu/ebookMLCB: ebook Machine Learning cơ bản](https://github.com/tiepvupsu/ebookMLCB)
- [Grokking Machine Learning - Luis G. Serrano](https://www.manning.com/books/grokking-machine-learning)
- [luisguiserrano/manning: Repository for the book Grokking Machine Learning, by Manning Editors](https://github.com/luisguiserrano/manning?tab=readme-ov-file)
- [Hands-on Machine Learning with Scikit-Learn, Keras](http://14.139.161.31/OddSem-0822-1122/Hands-On_Machine_Learning_with_Scikit-Learn-Keras-and-TensorFlow-2nd-Edition-Aurelien-Geron.pdf)
- [Introduction — Machine Learning from Scratch](https://dafriedman97.github.io/mlbook/content/introduction.html)
- [Introduction to Machine Learning](https://www.wolfram.com/language/introduction-machine-learning/)
- [Algorithms for Artificial Intelligence](https://web.stanford.edu/~mossr/pdf/alg4ai.pdf)
- [Brandon Rohrer](https://brandonrohrer.com/blog.html#193)
- [Introduction to Machine Learning with Python](https://www.nrigroupindia.com/e-book/Introduction%20to%20Machine%20Learning%20with%20Python%20(%20PDFDrive.com%20)-min.pdf)
- [1761295321783](https://media.licdn.com/dms/document/media/v2/D4D1FAQErMYEo3920aw/feedshare-document-pdf-analyzed/B4DZoVYVQZGwAc-/0/1761295321783?e=1762387200&v=beta&t=Qivb1ixvpVAlE5qlZeDJrvsGTmE0Hq4aZgGrbICMsNY&fbclid=IwY2xjawNsVaZleHRuA2FlbQIxMABicmlkETFNcWZySU9ySW1wRGVubXN4AR5Ep-OAT69ypIzhllIwnR96umb138DbmvFRgOxFbMEuq_xeH8ov0VBs3gBr6w_aem_ZVR5_rE7uKa2h4EmflepBg)
- [notes.pdf](https://marthawhite.github.io/mlcourse/notes.pdf)
- [2019BurkovTheHundred-pageMachineLearning.pdf](http://ema.cri-info.cm/wp-content/uploads/2019/07/2019BurkovTheHundred-pageMachineLearning.pdf)
- [The Hundred-Page Machine Learning Book by Andriy Burkov](https://themlbook.com/)
- [Contents (hardcover) [The Hundred-Page Machine Learning Book]](https://themlbook.com/wiki/doku.php?id=contents)
- [Machine Learning Handbook — Machine Learning Handbook](https://www.bpesquet.fr/mlhandbook/)
- [Papers-Literature-ML-DL-RL-AI/General-Machine-Learning at master · tirthajyoti/Papers-
- [https://media.licdn.com/dms/document/D4D1FAQG7JMpMEUNRnQ/feedshare-document-pdf-analyzed/0/1664549941323?e=1672876800&v=beta&t=PC0PML_TlgOJOuKvfaghEYVWqBD6hbpXDWUb1h4PeL8](https://media.licdn.com/dms/document/media/v2/D561FAQEatMaYJE-LCg/feedshare-document-pdf-analyzed/B56Zol6KTFI8Ac-/0/1761572602583?e=1762387200&v=beta&t=mb_nxKau4J34gMx8VZdlqxuwKZgY_XCoIKOjh7-l5MY&fbclid=IwY2xjawNteQhleHRuA2FlbQIxMABicmlkETEyOExhZ3dlWjAwQUpaT2g1AR5LgLghRhRouxSDfgL2TzHlgutf1_5hPcoNpAaaVI0LMsZQdhiD3nlWVt1q5g_aem_HfiQSJPBpwevcICChSNDFQ)
### Collections
- [linux08/machine-learning-books](https://github.com/linux08/machine-learning-books)
- [gimac/gninrael-enihcam: machine learning resources](https://github.com/gimac/gninrael-enihcam)
- [tim-hub/machine-learning-books: this is a collection of books and courses for machine learning.](https://github.com/tim-hub/machine-learning-books)
- [3_essential_books_for_ML - Google Drive](https://drive.google.com/drive/folders/1io-RxmKendqoEWyGnxfh9t2mIP1MN_NL?fbclid=IwY2xjawNVzoJleHRuA2FlbQIxMABicmlkETFiTEJsb0Z4OGhoQzFkYXBnAR5b1yi6u4pKLZsqplccQohf2g4N8oGUIKLUf1b_tbB11EQk1IzZ1y-9XntXwQ_aem_gAXVgxIXUdCZfS-o2kXdIQ)
- [Literature-ML-DL-RL-AI](https://github.com/tirthajyoti/Papers-Literature-ML-DL-RL-AI/tree/master/General-Machine-Learning)
- [harvard-edge/cs249r_book: Introduction to Machine Learning Systems](https://github.com/harvard-edge/cs249r_book)
## Lecture Notes
- [main_notes.pdf](https://cs229.stanford.edu/main_notes.pdf)
- [notes.pdf](https://www.cs.cmu.edu/~hn1/documents/machine-learning/notes.pdf)
- [6_390_lecture_notes_spring24.pdf](https://introml.mit.edu/_static/spring24/LectureNotes/6_390_lecture_notes_spring24.pdf)
- [Introduction to Machine Learning Lecture Notes for COS 324 at Princeton University](https://princeton-introml.github.io/files/COS324_Course_Notes.pdf)
- [CS229_Lecture_Notes.pdf](https://sgfin.github.io/files/notes/CS229_Lecture_Notes.pdf?fbclid=IwY2xjawGP9yVleHRuA2FlbQIxMAABHdMu8hRfI6QCAAv4vfCs1D8WpoTxc5Zbx6hMuUO75AlaWqrZGOmlkdv_DA_aem_rykgRXfhr0kOccFKLDIHDw)
- [Home | COS 324 Notes](https://princeton-introml.github.io/)
- [100 Lectures on Machine Learning (Mark Schmidt)](https://www.cs.ubc.ca/~schmidtm/Courses/LecturesOnML/)
- [Teaching - CS 229](https://stanford.edu/~shervine/teaching/cs-229/)
- [machlearn.pdf](https://people.eecs.berkeley.edu/~jrs/papers/machlearn.pdf)
- [10-301 + 10-601, Fall 2023](https://www.cs.cmu.edu/~mgormley/courses/10601-f23/schedule.html)
- [1909.03550](https://arxiv.org/pdf/1909.03550)
- [CS229br Foundations of Deep Learning (aka Topics in the Foundations of Machine Learning)](https://boazbk.github.io/mltheoryseminar/)
- [6.390 | IntroML | Fall25](https://introml.mit.edu/fall25)
- [Intro and Overview Machine Learning Lecture — Machine Learning Lecture](https://maucher.pages.mi.hdm-stuttgart.de/mlbook/intro.html)
## Repositories
- [AMAI-GmbH/AI-Expert-Roadmap: Roadmap to becoming an Artificial Intelligence Expert in 2022](https://github.com/AMAI-GmbH/AI-Expert-Roadmap)
- [josephmisiti/awesome-machine-learning: A curated list of awesome Machine Learning frameworks, libraries and software.](https://github.com/josephmisiti/awesome-machine-learning)
- [afshinea (Afshine Amidi)](https://github.com/afshinea)
- [Machine Learning Tokyo · GitHub](https://github.com/Machine-Learning-Tokyo)
- [Machine Learning For Everyone(ML4E)](https://github.com/Machine-Learning-for-Everyone-ML4E)
- [bangoc123/learn-machine-learning-in-two-months: Những kiến thức cần thiết để học tốt Machine Learning trong vòng 2 tháng. Essential Knowledge for learning Machine Learning in two months.](https://github.com/bangoc123/learn-machine-learning-in-two-months)
- [microsoft/AI-For-Beginners: 12 Weeks, 24 Lessons, AI for All!](https://github.com/microsoft/AI-For-Beginners/tree/main)
- [microsoft/ML-For-Beginners: 12 weeks, 26 lessons, 52 quizzes, classic Machine Learning for all](https://github.com/microsoft/ML-For-Beginners)
## Papers
- [dair-ai/ML-Papers-of-the-Week: 🔥Highlighting the top ML papers every week.](https://github.com/dair-ai/ML-Papers-of-the-Week)
- [Trending Papers - Hugging Face](https://huggingface.co/papers/trending)
- [Papertalk - the platform for scientific paper presentations](https://papertalk.org/index)
- [Explore | alphaXiv](https://www.alphaxiv.org/)
- [openreview.net](https://openreview.net/)
## Videos
-  [What is Artificial Intelligence? - YouTube](https://www.youtube.com/watch?v=S-Ekh642XVs)
- [The Most Important Algorithm in Machine Learning - YouTube](https://www.youtube.com/watch?v=SmZmBKc7Lrs&t=191s)
### Channels
- [ProtonX - YouTube](https://www.youtube.com/@ProtonX)
- [Edan Meyer - YouTube](https://www.youtube.com/@EdanMeyer)
- [Rajistics - data science, AI, and machine learning - YouTube](https://www.youtube.com/@Rajistics)
- [Two Minute Papers - YouTube](https://www.youtube.com/@TwoMinutePapers)
- [Welch Labs - YouTube](https://www.youtube.com/channel/UConVfxXodg78Tzh5nNu85Ew)
- [sentdex - YouTube](https://www.youtube.com/channel/UCfzlCWGWYyIQ0aLC5w48gBQ)
- [Visually Explained - YouTube](https://www.youtube.com/@VisuallyExplained)
- [hu-po - YouTube](https://www.youtube.com/@hu-po)
- [Emergent Garden - YouTube](https://www.youtube.com/@EmergentGarden)
- [Power H - YouTube](https://www.youtube.com/@powerh5888/featured)
- [Intuitive Machine Learning - YouTube](https://www.youtube.com/@IntuitiveMachineLearning)
- [3Blue1Brown - YouTube](https://www.youtube.com/@3blue1brown)
- [far1din - YouTube](https://www.youtube.com/@far1din)
- [Denis Dmitriev - YouTube](https://www.youtube.com/@DenisDmitrievDeepRobotics)
- [deeplizard - YouTube](https://www.youtube.com/deeplizard)
- [vcubingx - YouTube](https://www.youtube.com/@vcubingx)
- [StatQuest with Josh Starmer - YouTube](https://www.youtube.com/@statquest)
- [Artem Kirsanov - YouTube](https://www.youtube.com/@ArtemKirsanov)
- [Steve Brunton - YouTube](https://www.youtube.com/@Eigensteve)
- [AI Bites - YouTube](https://www.youtube.com/@AIBites)
- [BlackBoard AI - YouTube](https://www.youtube.com/@BlackBoardAI)
- [Deepia - YouTube](https://www.youtube.com/@Deepia-ls2fo)
- [DeepFindr - YouTube](https://www.youtube.com/@DeepFindr)
- [DeepBean - YouTube](https://www.youtube.com/@deepbean)
- [Underfitted - YouTube](https://www.youtube.com/@underfitted)
- [Great Fate - YouTube](https://www.youtube.com/@greatfate)
- [Paper in a Pod - YouTube](https://www.youtube.com/@PaperinaPod)
- [The AI Guy - YouTube](https://www.youtube.com/@TheAIGuyExplains)
### Playlists
- [C++ Machine Learning - YouTube](https://www.youtube.com/playlist?list=PL79n_WS-sPHKklEvOLiM1K94oJBsGnz71)
- [Artificial Intelligence - YouTube](https://www.youtube.com/playlist?list=PLbg3ZX2pWlgKV8K6bFJr5dhM7oOClExUJ)
- [Machine Learning - YouTube](https://www.youtube.com/playlist?list=PLfsEr6YiELAA7iZvtF5s_-2N36HpdqE6t)
## Interactive
- [MLU-Explain](https://mlu-explain.github.io/)
- [GitHub - Machine-Learning-Tokyo/Interactive_Tools: Interactive Tools for Machine Learning, Deep Learning and Math](https://github.com/Machine-Learning-Tokyo/Interactive_Tools)
## Communities
- [People + AI Research](https://pair.withgoogle.com/)
- [Kaggle: Your Machine Learning and Data Science Community](https://www.kaggle.com/)
- [Hugging Face – The AI community building the future.](https://huggingface.co/)
- [AI Summer | Learn Deep Learning and Artificial Intelligence](https://theaisummer.com/)
- [AI Folks - Learn AI and Data Science in 16 weeks](https://www.aifolks.org/)
- [AI, but simple](https://www.aibutsimple.com/)
- [Turing Post](https://www.turingpost.com/)
- [AI 2027](https://ai-2027.com/)
- [ML Code Challenges - Deep-ML](https://www.deep-ml.com/)
- [There's An AI For That | AI Database](https://theresanaiforthat.com/?ref=producthunt)
- [Distill — Latest articles about machine learning](https://distill.pub/)
## Blogs
- [Juergen Schmidhuber's home page - Universal Artificial Intelligence - AI - Deep Learning - Recurrent Neural Networks - Computer Vision - Object Detection - Image segmentation - GANs - Transformers with linearized self-attention - Goedel Machine - Theory of everything - Algorithmic theory of everything - Computable universe - Zuse's thesis - Universal learning algorithms - Universal search - Kolmogorov Complexity - Algorithmic information - Super Omega - Speed Prior - Independent component analysis - ICA - Financial forecasting - Evolution - Reinforcement learning - POMDPs - Reinforcement learning economy - Hierarchical learning - Metalearning - Learning to learn - Self-Improvement - Genetic programming - Attentive vision - Active exploration - Theory of beauty - Theory of creativity - Theory of Humor - Facial Attractiveness - Low-complexity Art - Lego Art](https://people.idsia.ch/~juergen/)
- [Polo Club of Data Science @ Georgia Tech: Human-Centered AI, Deep Learning Interpretation & Visualization, Cybersecurity, Large Graph Visualization and Mining | Georgia Tech | Atlanta, GA 30332, United States](https://poloclub.github.io/)
- [Lex Fridman](https://lexfridman.com/)
- [Home - colah's blog](http://colah.github.io/)
- [Survival Strategies for the Robot Rebellion](https://pjreddie.com/)
- [Professor Richard Zemel](https://www.cs.toronto.edu/~zemel/inquiry/home.php)
- [Alex L. Zhang](https://alexzhang13.github.io/)
- [Jonathan Y. Chan | jyc](https://www.jonathanychan.com/)
- [Boyang Deng](https://boyangdeng.com/)
- [Mia Tang](https://www.mia-tang.com/)
- [Guandao Yang](https://www.guandaoyang.com/)
- [Ben Hoover](https://bhoov.com/)
- [Boaz Barak](https://www.boazbarak.org/)
- [explained.ai](https://explained.ai/)
- [emilyreif.com](https://emilyreif.com/)
- [Machine Learning Fundamentals](https://ataspinar.com/)
- [while my_mcmc:  gently(samples) -](https://twiecki.io/)
- [Jorge Froilan Gimenez Perez | Software Engineer Resume | 호르헤](https://gimenezp.dev/)
- [(4) Victor (@victor_explore) / X](https://x.com/victor_explore)
- [adit.io](https://www.adit.io/index.html)
- [ōtoro.net](https://otoro.net/ml/)
- [home -](https://maelfabien.github.io/)
- [rodmar.dev](https://www.rodmar.dev/)
- [Ludwig - Home](https://ludwigabap.com/)
- [The Den](https://hy3na.com/index.html)
- [Denny's Blog](https://dennybritz.com/)
- [neuralnetwork](https://cneuralnets.netlify.app/)
- [vxnuaj](https://www.vxnuaj.com/)
- [Lil'Log](https://lilianweng.github.io/)
- [spike](https://supaiku.com/)
### Vietnamese
- [Khanh X. Nguyen](https://machineslearner.com/)
- [Chip Huyen](https://huyenchip.com/)
- [Khoa học dữ liệu](https://phamdinhkhanh.github.io/content)
- [Quy's blog](https://ndquy.github.io/)
- [ThetaLog](https://thetalog.com/)
- [Machine learning – Ông Xuân Hồng](https://ongxuanhong.wordpress.com/category/data-science/machine-learning/)

## Programming Libraries
- [scikit-learn: machine learning in Python — scikit-learn 1.5.1 documentation](https://scikit-learn.org/stable/index.html)
- [PyCaret Tutorial: A beginner's guide for automating ML workflows using PyCaret | DataCamp](https://www.datacamp.com/tutorial/guide-for-automating-ml-workflows-using-pycaret)
- [Gradio](https://gradio.app/)