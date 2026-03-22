# Awesome Neural Additive Models [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of papers, implementations, and resources related to **Neural Additive Models (NAMs)** and their variants — interpretable deep learning through additive structures.

Neural Additive Models combine the expressivity of neural networks with the interpretability of Generalized Additive Models (GAMs) by learning a linear combination of neural networks, each attending to a single input feature.

---

## Contents

- [Foundational Work](#foundational-work)
- [Architectural Extensions](#architectural-extensions)
  - [Higher-Order Interactions](#higher-order-interactions)
  - [Sparsity and Feature Selection](#sparsity-and-feature-selection)
  - [Bayesian and Uncertainty-Aware](#bayesian-and-uncertainty-aware)
  - [Distributional Regression (GAMLSS)](#distributional-regression-gamlss)
  - [Scalable Alternatives](#scalable-alternatives)
  - [Other Architectural Variants](#other-architectural-variants)
- [Neural GAM Alternatives](#neural-gam-alternatives)
- [Domain Applications](#domain-applications)
  - [Healthcare and Survival Analysis](#healthcare-and-survival-analysis)
  - [Finance and Credit Scoring](#finance-and-credit-scoring)
  - [Time Series and Forecasting](#time-series-and-forecasting)
  - [Scientific Discovery and Engineering](#scientific-discovery-and-engineering)
  - [Education](#education)
  - [Clustering](#clustering)
  - [Graph Data](#graph-data)
  - [Computer Vision](#computer-vision)
  - [Federated Learning](#federated-learning)
  - [Insurance and Actuarial](#insurance-and-actuarial)
  - [Speech and Language](#speech-and-language)
  - [Medical Imaging](#medical-imaging)
- [Theory and Analysis](#theory-and-analysis)
- [Surveys](#surveys)
- [Open-Source Implementations](#open-source-implementations)
  - [Official and Reference](#official-and-reference)
  - [PyTorch](#pytorch)
  - [R Packages](#r-packages)
  - [Libraries and Toolkits](#libraries-and-toolkits)
  - [NAM Variant Implementations](#nam-variant-implementations)
- [Tutorials and Blog Posts](#tutorials-and-blog-posts)
- [Benchmarks](#benchmarks)
- [Related Non-Neural GAMs](#related-non-neural-gams)

---

## Foundational Work

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2018 | **Explainable Neural Networks based on Additive Index Models (xNN)** | Vaughan, Sudjianto, Brahimi, Chen, Nair | arXiv | [Paper](https://arxiv.org/abs/1806.01933) |
| 2020 | **Adaptive Explainable Neural Networks (AxNN)** | Chen, Vaughan, Nair, Sudjianto | arXiv | [Paper](https://arxiv.org/abs/2004.02353) |
| 2021 | **Neural Additive Models: Interpretable Machine Learning with Neural Nets** | Agarwal, Melnick, Frosst, Zhang, Lengerich, Caruana, Hinton | NeurIPS 2021 | [Paper](https://arxiv.org/abs/2004.13912) · [Project](https://neural-additive-models.github.io/) · [Code](https://github.com/google-research/google-research/tree/master/neural_additive_models) |

---

## Architectural Extensions

### Higher-Order Interactions

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2022 | **Higher-Order Neural Additive Models (HONAM)** | Kim, Choi, Kim | IEEE 2022/2024 | [Paper](https://arxiv.org/abs/2209.15409) · [Code](https://github.com/gim4855744/HONAM) |
| 2022 | **Sparse Interaction Additive Networks (SIAN)** | Enouen, Liu | NeurIPS 2022 | [Paper](https://arxiv.org/abs/2209.09326) · [Code](https://github.com/EnouenJ/sparse-interaction-additive-networks) |
| 2024 | **Neural Additive and Basis Models with Feature Selection and Interactions** | Kishimoto, Yamanishi, Matsuda, Shirakawa | PAKDD 2024 | [Paper](https://link.springer.com/chapter/10.1007/978-981-97-2259-4_1) |
| 2025 | **Sparse Deep Additive Model with Interactions (SDAMI)** | Hung, Lin, Calhoun | arXiv 2025 | [Paper](https://arxiv.org/abs/2509.23068) |

### Sparsity and Feature Selection

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2023 | **Sparse Neural Additive Model (SNAM)** | Xu, Bu, Chaudhari, Barnett | ECML-PKDD 2023 | [Paper](https://arxiv.org/abs/2202.12482) |
| 2023 | **Structural Neural Additive Models** | Luber, Thielmann, Säfken | arXiv 2023 | [Paper](https://arxiv.org/abs/2302.09275) |

### Bayesian and Uncertainty-Aware

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2024 | **Improving Neural Additive Models with Bayesian Principles (LA-NAM)** | Bouchiat, Immer, Yèche, Rätsch, Fortuin | ICML 2024 | [Paper](https://arxiv.org/abs/2305.16905) · [Code](https://github.com/fortuinlab/LA-NAM) |
| 2024 | **Gaussian Process Neural Additive Models (GP-NAM)** | Zhang, Barr, Paisley | AAAI 2024 | [Paper](https://arxiv.org/abs/2402.12518) · [Code](https://github.com/Wei2624/GPNAM) |
| 2024 | **BayesNAM: Leveraging Inconsistency for Reliable Explanations** | Kim, Park, Choi, Lee, Lee | arXiv 2024 | [Paper](https://arxiv.org/abs/2411.06367) |
| 2026 | **EviNAM: Intelligibility and Uncertainty via Evidential Neural Additive Models** | Schleibaum, Thielmann, Teusch, Säfken, Müller | arXiv 2026 | [Paper](https://arxiv.org/abs/2601.08556) |

### Distributional Regression (GAMLSS)

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2024 | **Neural Additive Models for Location Scale and Shape (NAMLSS)** | Thielmann, Kruse, Kneib, Säfken | AISTATS 2024 | [Paper](https://arxiv.org/abs/2301.11862) · [Code](https://github.com/AnFreTh/NAMpy) |
| 2024 | **NODE-GAMLSS** | De, Thielmann, Säfken | NeurIPS 2024 Workshop | [Paper](https://openreview.net/forum?id=sWvTLlRkzy) |
| 2024 | **NBMLSS: Probabilistic Forecasting via Neural Basis Models for Location Scale and Shape** | Brusaferri, Ramin, Ballarino | arXiv 2024 | [Paper](https://arxiv.org/abs/2411.13921) |
| 2025 | **Quantile Neural Basis Models (QNBM)** | Brusaferri, Ramin, Ballarino | arXiv 2025 | [Paper](https://arxiv.org/abs/2509.14113) |

### Scalable Alternatives

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2022 | **NODE-GAM: Neural Generalized Additive Model for Interpretable Deep Learning** | Chang, Caruana, Goldenberg | ICLR 2022 (Spotlight) | [Paper](https://arxiv.org/abs/2106.01613) · [Code](https://github.com/zzzace2000/nodegam) |
| 2022 | **Neural Basis Models for Interpretability (NBM)** | Radenovic, Dubey, Mahajan | NeurIPS 2022 | [Paper](https://arxiv.org/abs/2205.14120) · [Code](https://github.com/facebookresearch/nbm-spam) |
| 2022 | **Scalable Interpretability via Polynomials (SPAM)** | Dubey, Radenovic, Mahajan | NeurIPS 2022 | [Paper](https://arxiv.org/abs/2205.14108) · [Code](https://github.com/facebookresearch/nbm-spam) |

### Other Architectural Variants

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2023 | **Generalizing Neural Additive Models via Statistical Multimodal Analysis (MNAM)** | Kim, Di Martino, Sapiro | ICML Workshop 2023 | [Paper](https://openreview.net/forum?id=xLg8ljlEba) · [Code](https://github.com/youngkyungkim93/MNAM) |
| 2024 | **ProtoNAM: Prototypical Neural Additive Models** | Xiong, Sinha, Zhang | ACM TKDD 2024 | [Paper](https://arxiv.org/abs/2410.04723) · [Code](https://github.com/teddy-xionggz/protonam) |
| 2024 | **GAMformer: In-Context Learning for Generalized Additive Models** | Mueller, Siems, Nori, Salinas, Zela, Caruana, Hutter | NeurIPS 2024 Workshop | [Paper](https://arxiv.org/abs/2410.04560) |
| 2024 | **DNAMite: Interpretable Calibrated Survival Analysis with Discretized Additive Models** | Van Ness, Block, Udell | arXiv 2024 | [Paper](https://arxiv.org/abs/2411.05923) |
| 2024 | **M-GAM: Interpretable Generalized Additive Models for Datasets with Missing Values** | McTavish, Donnelly, Seltzer, Rudin | NeurIPS 2024 | [Paper](https://arxiv.org/abs/2412.02646) |
| 2025 | **NAMformer: Beyond Black-Box Predictions in Tabular Transformer Networks** | Thielmann, Reuter, Säfken | arXiv 2025 | [Paper](https://arxiv.org/abs/2504.08712) · [Code](https://github.com/OpenTabular/NAMpy) |
| 2025 | **MT-NAM: An Efficient and Adaptive Model for Epileptic Seizure Detection** | Afzal, Cevher, Shoaran | arXiv 2025 | [Paper](https://arxiv.org/abs/2503.08251) |
| 2025 | **Interpretable Clinical Classification with Kolmogorov-Arnold Additive Models (KAAM)** | Almodovar, Apellaniz, Garrido, Fernandez-Salvador, Zazo, Parras | arXiv 2025 | [Paper](https://arxiv.org/abs/2509.16750) |
| 2026 | **Neural Additive Experts** | Xiong et al. | arXiv 2026 | [Paper](https://arxiv.org/abs/2602.10585) |

---

## Neural GAM Alternatives

These papers propose alternative neural network approaches to learning GAMs, distinct from the original NAM architecture.

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2021 | **GAMI-Net: Explainable Neural Network based on GAMs with Structured Interactions** | Yang, Zhang, Sudjianto | Pattern Recognition 2021 | [Paper](https://arxiv.org/abs/2003.07132) · [Code](https://github.com/SelfExplainML/GamiNet) |
| 2024 | **Interpretable Generalized Additive Neural Networks (IGANN)** | Kraus, Tschernutter, Weinzierl, Zschech | EJOR 2024 | [Paper](https://doi.org/10.1016/j.ejor.2023.06.032) · [Code](https://github.com/MathiasKraus/igann) |
| 2024 | **IGANN Sparse: Bridging Sparsity and Interpretability** | Stoecker, Hambauer, Zschech, Kraus | ECIS 2024 | [Paper](https://arxiv.org/abs/2403.11363) · [Code](https://github.com/MathiasKraus/igann) |
| 2024 | **neuralGAM: Explainable GANNs with Independent Neural Network Training** | Ortega-Fernandez, Sestelo, Villanueva | Statistics & Computing 2024 | [Paper](https://doi.org/10.1007/s11222-023-10320-5) · [Code (R)](https://github.com/inesortega/neuralGAM) · [Code (Python)](https://github.com/inesortega/pyNeuralGAM) |
| 2024 | **Achieving Interpretable ML by Functional Decomposition into Explainable Predictor Effects** | Kohler, Rügamer, Schmid | arXiv 2024 | [Paper](https://arxiv.org/abs/2407.18650) |
| 2024 | **Neural-ANOVA: Analytical Model Decomposition using Automatic Integration** | Limmer, Udluft, Otte | MLSP 2025 | [Paper](https://arxiv.org/abs/2408.12319) |
| 2025 | **neuralGAM: An R Package for Fitting Generalized Additive Neural Networks** | Ortega-Fernandez, Sestelo | arXiv 2025 | [Paper](https://arxiv.org/abs/2505.08610) · [Code](https://github.com/inesortega/neuralGAM) |
| 2025 | **Tensor Product Neural Networks for Functional ANOVA (ANOVA-TPNN)** | Park, Kong, Choi, Park, Kim | arXiv 2025 | [Paper](https://arxiv.org/abs/2502.15215) |

---

## Domain Applications

### Healthcare and Survival Analysis

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2022 | **SurvNAM: The Machine Learning Survival Model Explanation** | Utkin, Satyukov, Konstantinov | Neural Networks 2022 | [Paper](https://arxiv.org/abs/2104.08903) |
| 2022 | **Extending NAM for Survival Analysis with EHR Data (TimeNAM)** | Peroni, Kurban, Yang, Kim, Kang, Song | arXiv 2022 | [Paper](https://arxiv.org/abs/2211.07814) |
| 2023 | **CoxNAM: An Interpretable Deep Survival Analysis Model** | Xu, Guo | Expert Systems with Applications 2023 | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0957417423007200) |
| 2024 | **Towards Reducing Diagnostic Errors with Interpretable Risk Prediction** | McInerney, Dickinson, Flynn, Young, Young, van de Meent, Wallace | NAACL 2024 | [Paper](https://arxiv.org/abs/2402.10109) |
| 2024 | **CoxSENAM: Self-Explaining Neural Networks with Cox Proportional Hazards** | Alabdallah, Hamed, Ohlsson, Rognvaldsson, Pashami | arXiv 2024 | [Paper](https://arxiv.org/abs/2407.13849) |
| 2024 | **Optimized IGANN for Human Brain Diagnosis using Medical Imaging** | — | Knowledge-Based Systems 2024 | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0950705124014965) |
| 2025 | **CRISP-NAM: Competing Risks Interpretable Survival Prediction with NAMs** | Ramachandram, Raval | EXPLIMED @ ECAI 2025 | [Paper](https://arxiv.org/abs/2505.21360) |
| 2025 | **Interpretable Fine-Gray Deep Survival Model for Competing Risks** | Ramachandram, Loefler, Roberts, Verma, Norman, Razak, Pow, de Mestral | arXiv 2025 | [Paper](https://arxiv.org/abs/2511.12409) |
| 2025 | **ADHAM: Additive Deep Hazard Analysis Mixtures** | Ketenci, Jeanselme, Reyes Nieva, Joshi, Elhadad | arXiv 2025 | [Paper](https://arxiv.org/abs/2509.07108) |

### Finance and Credit Scoring

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2022 | **Monotonic Neural Additive Models for Credit Scoring** | Chen, Ye | ACM ICAIF 2022 | [Paper](https://arxiv.org/abs/2209.10070) |
| 2023 | **Monotonicity for AI Ethics and Society** | Chen, Ye | arXiv 2023 | [Paper](https://arxiv.org/abs/2301.07060) |
| 2025 | **SAINTNet: Sparse-Enhanced Additive Interaction Neural Network for Credit Decision** | Lan, Fan, Liu | Decision Support Systems 2025 | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0167923625001083) |

### Time Series and Forecasting

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2021 | **Neural Additive Vector Autoregression Models (NAVAR)** | Bussmann, Nys, Latré | Discovery Science 2021 | [Paper](https://arxiv.org/abs/2010.09429) · [Code](https://github.com/bartbussmann/NAVAR) |
| 2022 | **Neural Additive Models for Nowcasting** | Kim | arXiv 2022 | [Paper](https://arxiv.org/abs/2205.10020) |
| 2023 | **Neural Additive Time-Series Models (NATMs)** | Jo, Kim | Expert Systems with Applications 2023 | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0957417423008096) |
| 2024 | **FocusLearn: Fully-Interpretable, High-Performance Modular Neural Networks for Time Series** | Su, Kloukinas, Garcez | arXiv 2024 | [Paper](https://arxiv.org/abs/2311.16834) |
| 2025 | **Hierarchical Neural Additive Models for Demand Forecasts (HNAM)** | Feddersen, Cleophas | Int. Journal of Forecasting 2025 | [Paper](https://arxiv.org/abs/2404.04070) |

### Scientific Discovery and Engineering

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2023 | **NAM-CAM: Neural-Additive Models for Semi-analytic Descriptions of CAM Simulations** | Ditschuneit, Frenk, Frings, Rudel, Dietzel, Otterbach | FAIM 2023 | [Paper](https://link.springer.com/chapter/10.1007/978-3-031-38241-3_30) |
| 2024 | **Neural Term Structure of Additive Process for Option Pricing** | Lin, Liu | arXiv 2024 | [Paper](https://arxiv.org/abs/2408.01642) |

### Education

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2024 | **Explainable Automatic Grading with Neural Additive Models** | Condor, Pardos | AIED 2024 | [Paper](https://arxiv.org/abs/2405.00489) |

### Clustering

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2024 | **NeurCAM: Interpretable Neural Clustering via Additive Models** | Upadhya, Cohen | ECAI 2024 | [Paper](https://arxiv.org/abs/2408.13361) |

### Graph Data

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2024 | **Graph Neural Additive Networks (GNAN)** | Bechler-Speicher, Globerson, Gilad-Bachrach | NeurIPS 2024 | [Paper](https://arxiv.org/abs/2406.01317) · [Code](https://github.com/mayabechlerspeicher/Graph-Neural-Additive-Networks---GNAN) |
| 2025 | **Graph Mixing Additive Networks (GMAN)** | Bechler-Speicher, Zerio, Huri, Vestergaard, Gilad-Bachrach, Jess, Bhatt, Sazonovs | arXiv 2025 | [Paper](https://arxiv.org/abs/2509.23923) |
| 2025 | **Identifying Critical Phases for Disease Onset with Sparse Haematological Biomarkers** | Zerio, Bechler-Speicher, Jess, Sazonovs | arXiv 2025 | [Paper](https://arxiv.org/abs/2503.14561) |

### Computer Vision

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2024 | **Neural Additive Image Model: Interpretation through Interpolation** | Reuter, Thielmann, Säfken | arXiv 2024 | [Paper](https://arxiv.org/abs/2405.02295) |
| 2025 | **INAM: Image-Scale Neural Additive Models** | — | ESANN 2025 | [Paper](https://www.esann.org/sites/default/files/proceedings/2025/ES2025-54.pdf) |
| 2025 | **Interpretable Similarity of Synthetic Image Utility** | Gatoula, Dimas, Iakovidis | arXiv 2025 | [Paper](https://arxiv.org/abs/2512.17080) |

### Federated Learning

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2024 | **Multi-Level Additive Modeling for Structured Non-IID Federated Learning** | Chen, Zhou, Long, Ma, Jiang, Zhang | arXiv 2024 | [Paper](https://arxiv.org/abs/2405.16472) |
| 2025 | **FedNAMs: Performing Interpretability Analysis in Federated Learning Context** | Nanda, Balija, Sahoo | arXiv 2025 | [Paper](https://arxiv.org/abs/2506.17466) |
| 2025 | **FedNAM+: The FedNAM+ Conformal Revolution** | Balija, Nanda, Sahoo | arXiv 2025 | [Paper](https://arxiv.org/abs/2506.17872) |

### Insurance and Actuarial

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2025 | **An Interpretable Deep Learning Model for General Insurance Pricing (Actuarial NAM)** | Laub, Pho, Wong | arXiv 2025 | [Paper](https://arxiv.org/abs/2509.08467) |

### Speech and Language

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2024 | **Speech as a Biomarker for Disease Detection** | Botelho, Abad, Schultz, Trancoso | arXiv 2024 | [Paper](https://arxiv.org/abs/2409.10230) |

### Medical Imaging

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2025 | **LucidAtlas: Uncertainty-Aware, Covariate-Disentangled Atlas Representations** | Jiao, Bhamidi, Qu, Zdanski, Kimbell et al. | arXiv 2025 | [Paper](https://arxiv.org/abs/2502.08445) |

---

## Theory and Analysis

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2021 | **How Interpretable and Trustworthy are GAMs?** | Chang, Tan, Lengerich, Goldenberg, Caruana | KDD 2021 | [Paper](https://arxiv.org/abs/2006.06466) · [Code](https://github.com/zzzace2000/GAMs) |
| 2024 | **Challenging the Performance-Interpretability Trade-off** | Kruschel et al. | BISE 2024 | [Paper](https://arxiv.org/abs/2409.14429) |
| 2024 | **Challenges in Interpretability of Additive Models** | Zhang, Martinelli, John | XAI-IJCAI 2024 Workshop | [Paper](https://arxiv.org/abs/2504.10169) |
| 2024 | **Dual Feature-Based and Example-Based Explanation Methods** | Konstantinov, Kozlov, Kirpichenko, Utkin | arXiv 2024 | [Paper](https://arxiv.org/abs/2401.16294) |
| 2025 | **Additive Models Explained: A Computational Complexity Approach** | Bassan et al. | NeurIPS 2025 | [Paper](https://arxiv.org/abs/2510.21292) |
| 2025 | **Reluctant Interaction Inference after Additive Modeling** | Huang, Panigrahi, Yu, Bien | arXiv 2025 | [Paper](https://arxiv.org/abs/2506.01219) |
| 2025 | **Bayesian Neural Networks for Functional ANOVA Model** | Park, Kim, Lee, Shin, Kong, Kim | arXiv 2025 | [Paper](https://arxiv.org/abs/2510.00545) |
| 2025 | **CausalKANs: Interpretable Treatment Effect Estimation with Kolmogorov-Arnold Networks** | — | arXiv 2025 | [Paper](https://arxiv.org/abs/2509.22467) |
| 2026 | **Provably Explaining Neural Additive Models** | Bassan, Elboher, Ladner, Sahin, Kretinsky, Althoff, Katz | ICLR 2026 | [Paper](https://arxiv.org/abs/2602.17530) |
| 2026 | **Statistical Inference for Explainable Boosting Machines** | — | AISTATS 2026 | [Paper](https://arxiv.org/abs/2601.18857) |
| 2026 | **The Most Important Features in GAMs Might Be Groups of Features** | Bosschieter, Franca, Wolk, Wu, Mehta, Dehoney, Kiss, Baker, Zhao, Caruana, Pohl | Scientific Reports 2026 | [Paper](https://arxiv.org/abs/2506.19937) |

---

## Surveys

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2025 | **A Comprehensive Survey on Self-Interpretable Neural Networks** | Ji, Sun, Zhang, Wang, Zhuang, Gong, Shen, Qin, Zhu, Xiong | IEEE TNNLS 2025 | [Paper](https://arxiv.org/abs/2501.15638) · [Code](https://github.com/yangji721/Awesome-Self-Interpretable-Neural-Network) |
| 2026 | **Comparison of GAMs and Neural Networks in Applications: A Systematic Review** | Doohan, Kook, Burke | Expert Systems with Applications 2026 | [Paper](https://arxiv.org/abs/2510.24601) |

---

## Open-Source Implementations

### Official and Reference

| Name | Framework | Description |
|------|-----------|-------------|
| [google-research/neural_additive_models](https://github.com/google-research/google-research/tree/master/neural_additive_models) | TensorFlow | Official Google Research implementation |
| [nickfrosst/neural_additive_models](https://github.com/nickfrosst/neural_additive_models) | TensorFlow | Standalone fork by co-author Nick Frosst |
| [agarwl/neural_additive_models](https://github.com/agarwl/neural_additive_models) | TensorFlow | Author Rishabh Agarwal's repo |

### PyTorch

| Name | Description |
|------|-------------|
| [AmrMKayid/nam](https://github.com/AmrMKayid/nam) | Full-featured NAM library with config system and notebooks |
| [kherud/neural-additive-models-pt](https://github.com/kherud/neural-additive-models-pt) | Clean PyTorch re-implementation, pip installable (`nam-pt`) |
| [rish-16/nam-pytorch](https://github.com/rish-16/nam-pytorch) | Lightweight unofficial implementation |
| [lemeln/nam](https://github.com/lemeln/nam) | Multi-task NAM by co-author Levi Melnick |

### R Packages

| Name | Description |
|------|-------------|
| [inesortega/neuralGAM](https://github.com/inesortega/neuralGAM) | CRAN package with backfitting-based independent NN training |

### Libraries and Toolkits

| Name | Framework | Description |
|------|-----------|-------------|
| [udellgroup/dnamite](https://github.com/udellgroup/dnamite) | PyTorch | Scikit-learn-compatible NAMs for regression, classification, and survival analysis with built-in feature selection |
| [AnFreTh/NAMpy](https://github.com/AnFreTh/NAMpy) | PyTorch | Supports NAM, NAMLSS, NAMformer, and distributional regression with formula-based specification |
| [interpretml/interpret](https://github.com/interpretml/interpret) | Python/C++ | Microsoft's InterpretML with EBM (tree-based GAM cousin of NAM) |

### NAM Variant Implementations

| Name | Variant | Framework | Description |
|------|---------|-----------|-------------|
| [zzzace2000/nodegam](https://github.com/zzzace2000/nodegam) | NODE-GAM | PyTorch | Differentiable oblivious decision tree backbone, sklearn-compatible |
| [facebookresearch/nbm-spam](https://github.com/facebookresearch/nbm-spam) | NBM + SPAM | PyTorch | Meta's shared basis models (70× fewer params) and polynomial GAMs |
| [fortuinlab/LA-NAM](https://github.com/fortuinlab/LA-NAM) | LA-NAM | PyTorch | Bayesian NAM via Laplace approximation |
| [gim4855744/HONAM](https://github.com/gim4855744/HONAM) | HONAM | PyTorch | Higher-order interaction NAMs |
| [EnouenJ/sparse-interaction-additive-networks](https://github.com/EnouenJ/sparse-interaction-additive-networks) | SIAN | PyTorch | Sparse high-order interaction detection |
| [Wei2624/GPNAM](https://github.com/Wei2624/GPNAM) | GP-NAM | PyTorch | Gaussian Process NAMs |
| [teddy-xionggz/protonam](https://github.com/teddy-xionggz/protonam) | ProtoNAM | PyTorch | Prototypical NAMs |
| [youngkyungkim93/MNAM](https://github.com/youngkyungkim93/MNAM) | MNAM | — | Multimodal NAMs |
| [SelfExplainML/GamiNet](https://github.com/SelfExplainML/GamiNet) | GAMI-Net | PyTorch/TF | Structured interaction networks |
| [MathiasKraus/igann](https://github.com/MathiasKraus/igann) | IGANN | Python | Extreme learning machine-based GANNs |
| [bartbussmann/NAVAR](https://github.com/bartbussmann/NAVAR) | NAVAR | PyTorch | Additive VAR for causal discovery |
| [mayabechlerspeicher/GNAN](https://github.com/mayabechlerspeicher/Graph-Neural-Additive-Networks---GNAN) | GNAN | PyTorch Geometric | Graph Neural Additive Networks |

---

## Tutorials and Blog Posts

| Resource | Description | Links |
|----------|-------------|-------|
| NAM Project Page | Official page with slides and links | [Website](https://neural-additive-models.github.io/) |
| NAM Presentation Slides | Rich Caruana's presentation | [PDF](https://neural-additive-models.github.io/assets/nam_slides.pdf) |
| Interpretable Deep Learning for Tabular Data — Neural GAMs | Blog post covering NAM, NODE-GAM, and related approaches | [Medium](https://medium.com/@chkchang21/interpretable-deep-learning-models-for-tabular-data-neural-gams-500c6ecc0122) |
| Neural Basis Models for Interpretability | Explains NBM vs NAM | [Towards Data Science](https://towardsdatascience.com/neural-basis-models-for-interpretability-fd04ac958ff2/) |

---

## Benchmarks

| Name | Description |
|------|-------------|
| [facebookresearch/nbm-spam](https://github.com/facebookresearch/nbm-spam) | Compares NBM, SPAM against NAM, EBM, XGBoost, DNNs |
| [LeoGrin/tabular-benchmark](https://github.com/LeoGrin/tabular-benchmark) | "Why do tree-based models still outperform deep learning on tabular data?" |
| [dholzmueller/pytabkit](https://github.com/dholzmueller/pytabkit) | ML model benchmarking toolkit for tabular data |
| [InterpretML Benchmarks](https://github.com/interpretml/interpret/blob/master/benchmarks/) | EBM comparison notebooks |

---

## Related Non-Neural GAMs

> If you're interested in GAMs themselves, check out **[Awesome Generalized Additive Models](https://github.com/suanlab/Awesome-Generalized-Additive-Models)**.

| Year | Title | Authors | Venue | Links |
|------|-------|---------|-------|-------|
| 2013 | **Accurate Intelligible Models with Pairwise Interactions (GA²M / EBM)** | Lou, Caruana, Gehrke, Hooker | KDD 2013 | [Paper](https://www.cs.cornell.edu/~yinlou/papers/lou-kdd13.pdf) · [Code](https://github.com/interpretml/interpret) |
| 2021 | **TabNet: Attentive Interpretable Tabular Learning** | Arik, Pfister | AAAI 2021 | [Paper](https://arxiv.org/abs/1908.07442) · [Code](https://github.com/dreamquark-ai/tabnet) |

---

## Contributing

Contributions welcome! If you find a paper or implementation missing from this list, please open a pull request.

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
