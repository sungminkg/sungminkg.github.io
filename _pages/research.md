---
permalink: /research/
title: "Research"
author_profile: true
---


## 💡 Research Interests

My research focuses on building **trustworthy** LLMs. I mainly work on **uncertainty quantification (UQ)** in LLMs for reliable decision-making. Moving forward, I aim to extend my research in **reasoning** and **interpretability**, to better understand the internal mechanisms of large models and leverage these insights to enhance their reliability and safety. I am also interested in advancing these directions toward **multi-modal** and **multi-agent** systems, with the long-term goal of developing trustworthy agents that can operate safely and transparently in the real world. Besides, I have research experience in federated learning and parameter-efficient fine-tuning.

**1) Knowledge Conflict and Robust UQ**  
LLMs often rely on external retrieval systems or internet search to supplement their responses. However, when the model’s parametric knowledge contradicts the retrieved contextual information, knowledge conflicts arise, leading to unreliable or inconsistent outputs. I am interested in developing robust UQ methods that can detect and resolve such conflicts by quantifying the reliability of both the model’s internal and retrieved knowledge. Another direction of my work is improving the robustness of UQ under domain shifts and specialized settings such as legal, financial, and medical documents, where models face high uncertainty and limited data coverage.

**2) Trustworthy Multi-Agent Reasoning**  
Multi-agent collaboration offers a promising way to enhance reasoning and decision reliability by enabling models to interact, debate, and verify one another’s responses. I aim to explore uncertainty-aware guidance strategies that allow multiple agents to reason collectively and generate safe and interpretable answers. Ultimately, I seek to design trustworthy agent systems that can operate in high-stakes domains, capable of abstaining from answers when uncertain, performing self-evaluation, and engaging in dynamic, context-aware reasoning.

**3) Trustworthiness in Multi-modal Models**  
Multi-modal models integrate diverse information sources such as text, image, audio, and video, yet it is difficult to trace where uncertainty originates and how it propagates across modalities. I am interested in understanding how confidence arises within these systems and how different modalities contribute to final predictions. By decomposing multi-modal representations and analyzing hidden activations and attention maps, I aim to improve the interpretability and reliability of multi-modal reasoning systems. 


## 🔬 Research Experiences

**1) Trustworthy Machine Learning**  
I have primarily worked on **uncertainty quantification** for LLM-generated answers. I have explored how LLM UQ methods perform in realistic aspects, including threshold sensitivity, query transformations, long-form applicability, and ensemble effectiveness. Along with this work, I participated in building [**TruthTorchLM**](https://github.com/Ybakman/TruthTorchLM), an open-source library implementing 25+ UQ methods with unified evaluation, calibration, and long-form claim-level assessment. I also proposed a UQ method for contextual QA that measures feature gaps along honesty, contextual reliance, and context comprehension via contrastive prompts and representation analysis. Overall, I worked on a survey paper for LLM UQ for hallucination detection, providing comprehensive overview of LLM UQ and systematic categorization of existing methods with individual brief explanation. 

Selected Papers:
- [*Reconsidering LLM Uncertainty Estimation Methods in the Wild*](https://arxiv.org/abs/2506.01114), **ACL 2025** 
- [*TruthTorchLM: A Comprehensive Library for Predicting Truthfulness in LLM Outputs*](https://arxiv.org/abs/2507.08203), **EMNLP 2025** 
- [*Uncertainty Quantification for Hallucination Detection in Large Language Models: Foundations, Methodology, and Future Directions*](https://arxiv.org/abs/2510.12040) 
- [*Uncertainty as Feature Gaps: Epistemic Uncertainty Quantification of LLMs in Contextual Qusestion-Answering*](https://arxiv.org/abs/2510.02671) 

<br>

**2) Efficient and Scalable Machine Learning**  
I have worked in making machine learning systems more **efficient** and **scalable** through signal-driven methods. In particular, I introduced the use of the gradient-to-weight ratio as a measure to interpret how much each layer or parameter has learned relative to its weight. I proposed using a gradient-to-weight ratio and entropy-based masking method, achieving 1.5% higher accuracy than full fine-tuning with 0.1% tunable parameters. In addition, I developed a federated learning algorithm that selectively updates high-variability layers, reducing communication costs by up to 83% without loss in accuracy. 

Selected Papers:  
- [*Layer-wise Update Aggregation with Recycling for Communication-Efficient Federated Learning*](https://www.arxiv.org/abs/2503.11146), **NeurIPS 2025**
- [*GEM: A Scale- and Distribution-Aware Sparse Fine-Tuning Framework for Effective Downstream Adaptation*](https://arxiv.org/abs/2508.16191), preprint

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
