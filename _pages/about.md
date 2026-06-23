---
permalink: /
title: "About"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

Howdy! I'm an incoming Ph.D. student in Computer Science at [Texas A&M University](https://www.tamu.edu/), advised by Prof. [Zhengzhong Tu](https://vztu.github.io), starting in Fall 2026. Currently, I am working as a Research Intern in the Mathematics and Computer Science (MCS) Division at [Argonne National Laboratory](https://www.anl.gov/), where I work with Dr. [Kibaek Kim](https://kibaekkim.github.io).

Previously, I earned my master's degree in Electrical Engineering at the [University of Southern California](https://www.usc.edu/), where I closely worked with Prof. [Salman Avestimehr](https://www.avestimehr.com/) and Prof. [Sai Praneeth Karimireddy](https://spkreddy.org), and collaborated with Prof. [Sunwoo Lee](https://sites.google.com/view/sunwoolee/home). I received my B.S. in Electronic Engineering from [Sogang University](https://wwwe.sogang.ac.kr/), where I worked with Prof. [Hongseok Kim](https://nice.sogang.ac.kr/).

My research interests broadly span **Generative AI**, **Agentic AI**, **Multimodal AI**, and **Trustworthy AI**, with the goal of building practical AI systems that can be deployed in real-world settings. Rather than treating these areas as separate directions, I am especially interested in their intersection: how capable generative and agentic systems can reason over multimodal information while remaining reliable, interpretable, and safe.

My research experience includes:

- **Trustworthy LLMs:** LLM Uncertainty Quantification, Hallucination Detection, Representation Analysis and Control
- **Efficient Machine Learning:** Federated Learning, Distributed Systems, Parameter-Efficient Fine-Tuning (PEFT), Gradient-based Importance Estimation

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

# News

<div class="news-scroll">
<ul>
  <li><strong>Jun 08, 2026</strong> - I started my summer internship at <a href="https://www.anl.gov/">Argonne National Laboratory</a>, where I am working on asynchronous federated learning.</li>
  <li><strong>May 15, 2026</strong> - I graduated from the <a href="https://www.usc.edu">University of Southern California</a> with my M.S. in Electrical Engineering and was selected as an MS Honors Fellow.</li>
  <li><strong>May 07, 2026</strong> - Honored to receive the <strong>Outstanding Academic Achievement Award</strong> from the Ming Hsieh Department of Electrical and Computer Engineering at USC, awarded to one master's student in the department.</li>
  <li><strong>Apr 30, 2026</strong> - Our paper, <a href="https://ieeexplore.ieee.org/abstract/document/11512977"><em>Uncertainty Quantification for Hallucination Detection in Large Language Models: Foundations, Methodology, and Future Directions</em></a>, was accepted to <strong>IEEE BITS the Information Theory Magazine</strong>.</li>
  <li><strong>Jan 25, 2026</strong> - Our paper <a href="https://openreview.net/forum?id=OWvvdl27CE"><em>Uncertainty as Feature Gaps: Epistemic Uncertainty Quantification of LLMs in Contextual Question-Answering</em></a> got accepted to <strong>ICLR 2026</strong>.</li>
  <li><strong>Nov 07, 2025</strong> - My first first-author paper <a href="https://ojs.aaai.org/index.php/AAAI/article/view/39410"><em>GEM: A Scale-Aware and Distribution-Sensitive Sparse Fine-Tuning Framework for Effective Downstream Adaptation</em></a> was accepted to <strong>AAAI 2026</strong>.</li>
  <li><strong>Oct 31, 2025</strong> - Honored to receive the Best Poster Award at the USC ECE 15th Annual Research Festival, among 110 participating teams.</li>
  <li><strong>Sep 18, 2025</strong> - Our paper <a href="https://openreview.net/forum?id=t6EPMcudln"><em>Layer-wise Update Aggregation with Recycling for Communication-Efficient Federated Learning</em></a> got accepted to <strong>NeurIPS 2025</strong>.</li>
  <li><strong>Sep 10, 2025</strong> - Our <a href="https://aclanthology.org/2025.emnlp-demos.54/"><em>TruthTorchLM</em></a> paper got accepted to <strong>EMNLP 2025 System Demonstrations</strong>.</li>
  <li><strong>May 15, 2025</strong> - Our paper <a href="https://aclanthology.org/2025.acl-long.1429/"><em>Reconsidering LLM Uncertainty Estimation Methods in the Wild</em></a> was accepted to <strong>ACL 2025</strong>.</li>
</ul>
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

Feel free to contact me at [sungmin.kang@tamu.edu](mailto:sungmin.kang@tamu.edu) or connect via [LinkedIn](https://www.linkedin.com/in/sungmin-kang-1999y64/). My CV is available [here]({{ site.baseurl }}/assets/CV_Sungmin_Kang.pdf).
