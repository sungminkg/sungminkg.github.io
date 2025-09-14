---
permalink: /research/
title: "Research"
author_profile: true
---


## 🔬 Research Interest  

My research focuses on building **trustworthy** and **scalable** machine learning systems, with applications to large language models (LLMs) and distributed learning.  

**1) Trustworthy Machine Learning**  
I am particularly interested in **uncertainty quantification (UQ)** for LLMs, aiming to improve interpretability and reliability. My interests include:  
- **Knowledge conflict**: quantifying uncertainty when contextual information contradicts parametric knowledge.  
- **Interpretability**: leveraging hidden representations and attention maps for UQ and explanation.  
- **Robustness**: addressing domain shifts and distributional changes.  
- **Applications**: hallucination detection and uncertainty-aware adaptive guidance for reasoning in LLMs.  

Representative papers:  
- [*Reconsidering LLM Uncertainty Estimation Methods in the Wild*](https://arxiv.org/abs/2506.01114), **ACL 2025** – Explored the behavior of LLM uncertainty estimation methods across threshold sensitivity, query transformations, long-form applicability, and ensemble effectiveness.  
- [*TruthTorchLM: A Comprehensive Library for Predicting Truthfulness in LLM Outputs*](https://arxiv.org/abs/2507.08203), **EMNLP 2025** – Released [**TruthTorchLM**](https://github.com/Ybakman/TruthTorchLM), an open-source library implementing 30+ truthfulness prediction methods with unified evaluation, calibration, and long-form claim-level assessment.  

**2) Efficient and Adaptive Machine Learning**  
Beyond trustworthiness, I am also interested in making learning systems more **efficient** and **adaptive** by exploiting signal-driven methods. My interests include:  
- **Learning with gradient signals**: improving generalization and reducing cost via parameter selection based on gradient-to-weight ratios.  
- **Reducing communication/computation**: designing scalable algorithms for federated and distributed learning.  
- **Mitigating client drift**: leveraging adaptive update strategies to stabilize decentralized training.  

Representative papers:  
- [*GEM: A Scale- and Distribution-Aware Sparse Fine-Tuning Framework for Effective Downstream Adaptation*](https://www.arxiv.org/abs/2503.11146), preprint – Proposed a gradient-to-weight ratio and entropy-based masking method, achieving 1.5% higher accuracy than full fine-tuning with 0.1% tunable parameters.  
- [*Layer-wise Update Aggregation with Recycling for Communication-Efficient Federated Learning*](https://www.arxiv.org/abs/2503.11146), preprint – Developed a federated learning algorithm that selectively updates high-variability layers, reducing communication costs by up to 83% without loss in accuracy.  






<!--
---
## 🌱 Ongoing Research (Coming soon!)

**Scale-Aware and Distribution-Sensitive Fine-Tuning**  
A parameter scale-aware and layer distribution-sensitive parameter-efficient fine-tuning framework

**In-Context Uncertainty Estimation**  
Uncertainty Quantification on knowledge conflict scenarios

**Foundational Modeling for AC-OPF with Federated Learning**  
Building a foundational GNN-based model for solving AC Optimal Power Flow (AC-OPF) problems using federated learning
-->
