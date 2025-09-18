---
permalink: /research/
title: "Research"
author_profile: true
---


## 🔬 Research Interest  

My research focuses on building **trustworthy** and **scalable** machine learning systems, with applications to large language models (LLMs) and decentralized learning.  

**1) Trustworthy Machine Learning**  
My primary research interest lies in **uncertainty quantification (UQ)** for LLM-generated answers, with the goal of improving both **reliability** and **interpretability**. In particular, I am interested in studying how uncertainty can capture **knowledge conflict**, when contextual information contradicts the model’s parametric knowledge. I am also excited about exploring interpretability by leveraging hidden representations and attention maps to better understand model behavior and support UQ. Another important direction of UQ is **robustness**, where I aim to design UQ methods that perform well under domain shifts and across specialized tasks such as legal, financial, and medical documents. Finally, I aim to extend UQ to **practical applications**, including hallucination detection and the development of uncertainty-aware guidance strategies to improve reasoning in LLMs.

Representative papers:  
- [*Reconsidering LLM Uncertainty Estimation Methods in the Wild*](https://arxiv.org/abs/2506.01114), **ACL 2025** – Explored the behavior of LLM uncertainty estimation methods across threshold sensitivity, query transformations, long-form applicability, and ensemble effectiveness.  
- [*TruthTorchLM: A Comprehensive Library for Predicting Truthfulness in LLM Outputs*](https://arxiv.org/abs/2507.08203), **EMNLP 2025** – Released [**TruthTorchLM**](https://github.com/Ybakman/TruthTorchLM), an open-source library implementing 30+ truthfulness prediction methods with unified evaluation, calibration, and long-form claim-level assessment.  

<br>

**2) Efficient and Scalable Machine Learning**  
Beyond trustworthiness, I am also interested in making learning systems more **efficient** and **scalable** through signal-driven methods. In particular, I study how gradient information can be used to prioritize important parameters for **task adaptation** and how gradients can be recycled to reduce communication costs in **federated learning**. Furthermore, I aim to develop adaptive update strategies to **mitigate client drift**, thereby improving global generalization in decentralized training while maintaining efficiency.

Representative papers:  
- [*Layer-wise Update Aggregation with Recycling for Communication-Efficient Federated Learning*](https://www.arxiv.org/abs/2503.11146), **NeurIPS 2025** – Developed a federated learning algorithm that selectively updates high-variability layers, reducing communication costs by up to 83% without loss in accuracy.  
- [*GEM: A Scale- and Distribution-Aware Sparse Fine-Tuning Framework for Effective Downstream Adaptation*](https://arxiv.org/abs/2508.16191), preprint – Proposed a gradient-to-weight ratio and entropy-based masking method, achieving 1.5% higher accuracy than full fine-tuning with 0.1% tunable parameters.  

---



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
