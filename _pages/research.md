---
permalink: /research/
title: "Research"
author_profile: true
---


## 🔬 Research Interest  

My research focuses on building trustworthy LLMs. I mainly work on uncertainty quantification in LLMs for reliable decision-making. Moving forward, I aim to extend my research in reasoning and interpretability, to better understand the internal mechanisms of large models and leverage these insights to enhance their reliability and safety. I am also interested in advancing these directions toward multi-modal and multi-agent systems, with the long-term goal of developing trustworthy agents that can operate safely and transparently in the real world. Besides, I have research experience in federated learning and parameter-efficient fine-tuning.




## 🔬 Research Experiences

**1) Trustworthy Machine Learning**  
My primary research interest lies in **uncertainty quantification (UQ)** for LLM-generated answers, with the goal of improving both **reliability** and **interpretability**. In particular, I am interested in UQ under **knowledge conflicts**, when the model’s parametric knowledge contradicts the contextual information. I am also excited about exploring interpretability by leveraging hidden representations and attention maps to better understand model behavior and support UQ. Another important direction of UQ is **robustness**, where I aim to design UQ methods that perform well under domain shifts and across specialized tasks such as legal, financial, and medical documents. Finally, I aim to extend UQ to **practical applications**, including hallucination detection and the development of uncertainty-aware guidance strategies to improve reasoning in LLMs.

Selected Papers:
- [*Reconsidering LLM Uncertainty Estimation Methods in the Wild*](https://arxiv.org/abs/2506.01114), **ACL 2025** – Explored the behavior of LLM uncertainty estimation methods across threshold sensitivity, query transformations, long-form applicability, and ensemble effectiveness.  
- [*TruthTorchLM: A Comprehensive Library for Predicting Truthfulness in LLM Outputs*](https://arxiv.org/abs/2507.08203), **EMNLP 2025** – Released [**TruthTorchLM**](https://github.com/Ybakman/TruthTorchLM), an open-source library implementing 30+ truthfulness prediction methods with unified evaluation, calibration, and long-form claim-level assessment.
- [*Uncertainty Quantification for Hallucination Detection in Large Language Models: Foundations, Methodology, and Future Directions*](https://arxiv.org/abs/2510.12040) - A comprehensive overview of LLM uncertainty quantification, and how it can be used to understand and detect hallucinations in LLMs.
- [*Uncertainty as Feature Gaps: Epistemic Uncertainty Quantification of LLMs in Contextual Qusestion-Answering*](https://arxiv.org/abs/2510.02671) -Proposed a UQ method for contextual QA that measures feature gaps along honesty, contextual reliance, and context comprehension via contrastive prompts and representation analysis.

<br>

**2) Efficient and Scalable Machine Learning**  
I have worked in making machine learning systems more **efficient** and **scalable** through signal-driven methods. In particular, I studied how gradient information can be used to prioritize important parameters for fine-tuning and how gradients can be recycled to reduce communication costs in **federated learning**.

Selected Papers:  
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
