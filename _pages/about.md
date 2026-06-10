---
permalink: /
title: "About"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

Hi! I’m a 2nd-year Master's student in Electrical Engineering at the [University of Southern California](https://www.usc.edu/), working closely with Prof. [Salman Avestimehr](https://www.avestimehr.com/) and Prof. [Sai Praneeth Karimireddy](https://spkreddy.org). I also collaborate with Prof. [Sunwoo Lee](https://sites.google.com/view/sunwoolee/home). Previously, I received my B.S. in Electronic Engineering from [Sogang University](https://wwwe.sogang.ac.kr/), where I worked with Prof. [Hongseok Kim](https://nice.sogang.ac.kr/). In Summer 2026, I will work as a **research intern** at **Argonne National Laboratory**.

My research focuses on building **trustworthy LLMs**. I mainly work on **uncertainty quantification** in LLMs for reliable decision-making. Moving forward, I aim to extend my research in **reasoning** and **interpretability**, to better understand the internal mechanisms of large models and leverage these insights to enhance their reliability and safety. I am also interested in advancing these directions toward multi-modal and multi-agent systems, with the long-term goal of developing trustworthy agents that can operate safely and transparently in the real world. Besides, I have research experience in **federated learning** and **parameter-efficient fine-tuning**.

# News

- **Jan 25, 2026** - Our paper [*Uncertainty as Feature Gaps: Epistemic Uncertainty Quantification of LLMs in Contextual Question-Answering*](https://arxiv.org/abs/2510.02671) got accepted to **ICLR 2026**.
- **Jan 25, 2026** - I will be joining **Argonne National Laboratory** as a research intern this summer, working on large-scale heterogeneous federated learning as part of the **GENESIS project**.
- **Nov 07, 2025** - My first first-author paper [*GEM: A Scale-Aware and Distribution-Sensitive Sparse Fine-Tuning Framework for Effective Downstream Adaptation*](https://arxiv.org/abs/2508.16191) was accepted to **AAAI 2026**.
- **Oct 31, 2025** - Honored to receive the Best Poster Award at the USC ECE 15th Annual Research Festival, among 110 participating teams.
- **Oct 15, 2025** - Our survey paper [*Uncertainty Quantification for Hallucination Detection in Large Language Models: Foundations, Methodology, and Future Directions*](https://arxiv.org/abs/2510.12040) is released.
- **Sep 18, 2025** - Our paper [*Layer-wise Update Aggregation with Recycling for Communication-Efficient Federated Learning*](https://arxiv.org/abs/2503.11146) got accepted to **NeurIPS 2025**.
- **Sep 10, 2025** - Our [*TruthTorchLM*](https://arxiv.org/abs/2507.08203) paper got accepted to **EMNLP 2025 System Demonstrations**.
- **Jul 30, 2025** - I presented our paper, *Reconsidering LLM Uncertainty Estimation Methods in the Wild*, at **ACL 2025**.

# Work Experience

<div class="work-list">
  {% for w in site.data.work %}
    {% include work-item.html
       logo=w.logo company=w.company role=w.role tenure=w.tenure location=w.location %}
  {% endfor %}
</div>

# Publications

<div class="pub-container">
  <input type="radio" id="tab-selected" name="pub-tabs" checked>
  <input type="radio" id="tab-all" name="pub-tabs">

  <div class="pub-tabs">
    <label for="tab-selected" class="tab-btn btn-sel">Selected</label>
    <label for="tab-all" class="tab-btn btn-all">All Publications</label>
  </div>

  <div class="pub-list-wrapper selected-list">
    <div class="pub-list">
      {% for p in site.data.selected_publications %}
        {% include pub-item.html
          title=p.title
          authors=p.authors_html
          venue=p.venue
          badge=p.badge
          paper_url=p.paper_url
          code_url=p.code_url
          project_url=p.project_url
          dataset_url=p.dataset_url %}
      {% endfor %}
    </div>
  </div>

  <div class="pub-list-wrapper all-list">
    <div class="pub-list">
      {% for p in site.data.all_publications %}
        {% include pub-item.html
          title=p.title
          authors=p.authors_html
          venue=p.venue
          badge=p.badge
          paper_url=p.paper_url
          code_url=p.code_url
          project_url=p.project_url
          dataset_url=p.dataset_url %}
      {% endfor %}
    </div>
  </div>
</div>

# Selected Honors & Awards

<div class="award-list">
  {% for h in site.data.honors %}
    {% include honor-item.html
      title=h.title
      assoc=h.assoc
      desc=h.desc
      date=h.date %}
  {% endfor %}
</div>

# Education

<div class="edu-list">
  {% for e in site.data.edu %}
    {% include edu-item.html
      school=e.school
      degree=e.degree
      dept=e.dept
      period=e.period %}
  {% endfor %}
</div>

# Contact

Feel free to contact me at [kangsung@usc.edu](mailto:kangsung@usc.edu) or connect via [LinkedIn](https://www.linkedin.com/in/sungmin-kang-1999y64/). My CV is available [here]({{ site.baseurl }}/assets/CV_Sungmin_Kang.pdf).
