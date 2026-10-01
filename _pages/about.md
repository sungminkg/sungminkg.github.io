---
permalink: /
title: "About"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

Howdy! I'm a first year Ph.D. student in Computer Science at [Texas A&M University](https://www.tamu.edu/), advised by Prof. [Zhengzhong Tu](https://vztu.github.io).

Previously, I earned my master's degree in Electrical Engineering at the [University of Southern California](https://www.usc.edu/), where I closely worked with Prof. [Salman Avestimehr](https://www.avestimehr.com/) and Prof. [Sai Praneeth Karimireddy](https://spkreddy.org), also collaborating with Prof. [Sunwoo Lee](https://sites.google.com/view/sunwoolee/home). I worked as a Research Intern in the Mathematics and Computer Science (MCS) Division at [Argonne National Laboratory](https://www.anl.gov/), supervised by Dr. [Kibaek Kim](https://kibaekkim.github.io). I received my B.S. in Electronic Engineering from [Sogang University](https://wwwe.sogang.ac.kr/), where I worked with Prof. [Hongseok Kim](https://nice.sogang.ac.kr/).

My research focuses on **AI safety** and **Agentic AI**. As AI agents are given more autonomy and access, ensuring that they behave safely becomes crucial. At the same time, I believe today's foundation models are already highly capable, and much of the remaining gap lies in how we use them: how we structure agents, what information each one sees, and what they remember over time.

**AI Safety**

- **Web agent safety**: How visual and textual signals in web pages can steer or mislead screenshot-based agents, and how to measure and defend against such manipulation.

**Agentic AI**

- **Scalable agentic memory: learning to forget**: As agents operate over long horizons and learn continually, context keeps accumulating. Compression and efficiency help, but to scale, agents also need to decide what to remove: outdated or stale information that no longer helps, or even actively hurts.
- **Information flow in multi-agent systems**: Splitting a task across specialized agents with separate inputs lowers cost and contains failures, but it also creates information bottlenecks that can prevent the system from reaching its goal. Giving every agent the full context avoids this, but then the system starts to resemble a single prompted model. I want to understand where the right balance lies, and how to design agent systems that are both effective and safe.

I'm always happy to chat and collaborate. If any of these directions resonate with you, feel free to reach out!

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
  <li><strong>Aug 24, 2026</strong> - Started my Ph.D. journey at TAMU! </li>
  <li><strong>Jun 08, 2026</strong> - I started my summer internship at <a href="https://www.anl.gov/">Argonne National Laboratory</a>, working on agentic paper coder and asynchronous federated learning simulator.</li>
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
