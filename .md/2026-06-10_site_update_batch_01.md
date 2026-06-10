# Website Update Batch 01

Status: Applied to the live site source on 2026-06-10. Ready for build verification and push.

Workspace: `/home/kangsung/website`

## 1. Sidebar / Author Profile

Target file: `_config.yml`

Update:

```yaml
author:
  bio: "Incoming CS Ph.D. Student at Texas A&M University"
  location: "Lemont"
  employer: "Argonne National Laboratory"
  email: "kangsung@usc.edu"
```

Keep:

- Name: Sungmin Kang
- Pronouns: he/him/his
- Email: kangsung@usc.edu
- GitHub, Google Scholar, LinkedIn links
- Profile photo

## 2. About Section

Target file: `_pages/about.md`

Replace the current opening biography with this polished version:

```markdown
Hi! I'm an incoming Ph.D. student in Computer Science at [Texas A&M University](https://www.tamu.edu/), advised by Prof. [Zhengzhong Tu](https://vztu.github.io), starting in Fall 2026. Currently, I am working as a Research Intern in the Mathematical and Computer Science (MCS) Division at [Argonne National Laboratory](https://www.anl.gov/), where I work with Dr. [Kibaek Kim](https://kibaekkim.github.io).

Previously, I earned my master's degree in Electrical Engineering at the [University of Southern California](https://www.usc.edu/), where I closely worked with Prof. [Salman Avestimehr](https://www.avestimehr.com/) and Prof. [Sai Praneeth Karimireddy](https://spkreddy.org), and collaborated with Prof. [Sunwoo Lee](https://sites.google.com/view/sunwoolee/home). I received my B.S. in Electronic Engineering from [Sogang University](https://wwwe.sogang.ac.kr/), where I worked with Prof. [Hongseok Kim](https://nice.sogang.ac.kr/).
```

Replace the current research paragraph with this:

```markdown
My research interests broadly span **Generative AI**, **Agentic AI**, **Multimodal AI**, and **Trustworthy AI**, with the goal of building practical AI systems that can be deployed in real-world settings. Rather than treating these areas as separate directions, I am especially interested in their intersection: how capable generative and agentic systems can reason over multimodal information while remaining reliable, interpretable, and safe.

My research experience includes:

- **Trustworthy LLMs:** LLM Uncertainty Quantification, Hallucination Detection, Representation Analysis and Control
- **Efficient Machine Learning:** Federated Learning, Distributed Systems, Parameter-Efficient Fine-Tuning (PEFT), Gradient-based Importance Estimation
```

## 3. Section Order

Target file: `_pages/about.md`

New homepage order:

1. About
2. Work Experience
3. Publications
4. News
5. Selected Honors & Awards
6. Education
7. Contact

Notes:

- Move Work Experience immediately below About.
- Move News below Publications.

## 4. Browser Tab Icon / Favicon

Target files:

- `_includes/head/custom.html`
- `images/favicon.ico`
- `images/favicon-32x32.png`
- `images/favicon-192x192.png`
- `images/apple-touch-icon-180x180.png`
- `images/manifest.json`

Requested change:

- Replace the current favicon/icon set with Texas A&M University branding.
- USC-related icon assets can be removed if unused.

Source to use:

- Official Texas A&M favicon download page: `https://marcomm.tamu.edu/template/web-favicons/`
- Official direct template page found: `https://marcomm.tamu.edu/template_download/web-favicons/`

Implementation note:

- Download the official TAMU favicon PNG/ICO collection when applying the batch.
- Update `_includes/head/custom.html` so the browser tab icon points only to the new TAMU favicon files.
- Keep the site title as `Sungmin Kang`.

## 5. Work Experience

Target files:

- `_data/work.yml`
- `_includes/work-item.html` only if layout adjustment is needed

Update the ANL entry:

```yaml
- company: Argonne National Laboratory
  role: Research Intern
  tenure: "2026.06 - 2026.08"
  location: Lemont, IL, USA
  logo: /images/argonne-logo.png
```

Remove:

- `GENESIS Project`
- `Summer 2026`

Add:

- Argonne National Laboratory logo image.

Source:

- Prefer an official Argonne logo asset from `anl.gov` when implementing.

## 6. Publications

Target files:

- `_data/selected_publications.yml`
- `_data/all_publications.yml`

Keep:

- Selected Publications and All Publications identical for now.

Venue update:

```yaml
title: "Uncertainty Quantification for Hallucination Detection in Large Language Models: Foundations, Methodology, and Future Directions"
venue: "IEEE BITS the Information Theory Magazine 2025"
```

Official links found:

```yaml
- title: "Uncertainty as Feature Gaps: Epistemic Uncertainty Quantification of LLMs in Contextual Question-Answering"
  official_url: https://openreview.net/forum?id=OWvvdl27CE
  note: ICLR/OpenReview official page found.

- title: "GEM: A Scale-Aware and Distribution-Sensitive Sparse Fine-Tuning Framework for Effective Downstream Adaptation"
  official_url: https://ojs.aaai.org/index.php/AAAI/article/view/39410
  note: AAAI OJS official page found.

- title: "Layer-wise Update Aggregation with Recycling for Communication-Efficient Federated Learning"
  official_url: https://openreview.net/forum?id=t6EPMcudln
  note: NeurIPS/OpenReview official page found.

- title: "TruthTorchLM: A Comprehensive Library for Predicting Truthfulness in LLM Outputs"
  official_url: https://aclanthology.org/2025.emnlp-demos.54/
  code_url: https://github.com/Ybakman/TruthTorchLM
  note: ACL Anthology official page found.

- title: "Reconsidering LLM Uncertainty Estimation Methods in the Wild"
  official_url: https://aclanthology.org/2025.acl-long.1429/
  note: ACL Anthology official page found.
```

Official link still needs confirmation:

```yaml
- title: "Uncertainty Quantification for Hallucination Detection in Large Language Models: Foundations, Methodology, and Future Directions"
  current_url: https://ieeexplore.ieee.org/abstract/document/11512977
  requested_venue: "IEEE BITS the Information Theory Magazine 2025"
  note: Search found venue evidence but no stable official IEEE BITS article URL yet. Keep arXiv until official URL is provided or discoverable.
```

## 7. News

Target file: `_pages/about.md`

Requested behavior:

- Show News as a scrollable section.
- Display roughly 8 items in the visible area.
- Add local scroll inside the News block so older items can still be viewed.

Implementation idea:

```html
<div class="news-scroll">
  <ul>
    ...
  </ul>
</div>
```

Add CSS in the site Sass:

```scss
.news-scroll {
  max-height: 22rem;
  overflow-y: auto;
  padding-right: 0.75rem;
}
```

New / changed news items:

```markdown
- **Jun 08, 2026** - I started my summer internship at [Argonne National Laboratory](https://www.anl.gov/), where I am working on asynchronous federated learning.
- **May 15, 2026** - I graduated from the [University of Southern California](https://www.usc.edu) with my M.S. in Electrical Engineering and was selected as an MS Honors Fellow.
- **May 07, 2026** - Honored to receive the **Outstanding Academic Achievement Award** from the Ming Hsieh Department of Electrical and Computer Engineering at USC, awarded to one master's student in the department.
- **Apr 30, 2026** - Our paper, [*Uncertainty Quantification for Hallucination Detection in Large Language Models: Foundations, Methodology, and Future Directions*](https://ieeexplore.ieee.org/abstract/document/11512977), was accepted to **IEEE BITS the Information Theory Magazine**.
- **Jan 25, 2026** - Our paper [*Uncertainty as Feature Gaps: Epistemic Uncertainty Quantification of LLMs in Contextual Question-Answering*](https://openreview.net/forum?id=OWvvdl27CE) got accepted to **ICLR 2026**.
- **Nov 07, 2025** - My first first-author paper [*GEM: A Scale-Aware and Distribution-Sensitive Sparse Fine-Tuning Framework for Effective Downstream Adaptation*](https://ojs.aaai.org/index.php/AAAI/article/view/39410) was accepted to **AAAI 2026**.
- **Oct 31, 2025** - Honored to receive the Best Poster Award at the USC ECE 15th Annual Research Festival, among 110 participating teams.
- **Sep 18, 2025** - Our paper [*Layer-wise Update Aggregation with Recycling for Communication-Efficient Federated Learning*](https://openreview.net/forum?id=t6EPMcudln) got accepted to **NeurIPS 2025**.
- **Sep 10, 2025** - Our [*TruthTorchLM*](https://aclanthology.org/2025.emnlp-demos.54/) paper got accepted to **EMNLP 2025 System Demonstrations**.
- **May 15, 2025** - Our paper [*Reconsidering LLM Uncertainty Estimation Methods in the Wild*](https://aclanthology.org/2025.acl-long.1429/) was accepted to **ACL 2025**.
```

Remove:

```markdown
- **Jan 25, 2026** - I will be joining **Argonne National Laboratory** as a research intern this summer, working on large-scale heterogeneous federated learning as part of the **GENESIS project**.
- **Jul 30, 2025** - I presented our paper, *Reconsidering LLM Uncertainty Estimation Methods in the Wild*, at **ACL 2025**.
```

## 8. Selected Honors & Awards

Target file: `_data/honors.yml`

Use Haebin-style item formatting already present in the site.

Replace current honors with:

```yaml
- title: MS Honors Fellowship
  assoc: USC
  desc: Awarded for an excellent academic record and research achievements.
  date: "2026.05"

- title: Outstanding Academic Achievement Award
  assoc: USC Viterbi
  desc: Awarded to one master's student from the Ming Hsieh Department of Electrical and Computer Engineering.
  date: "2026.05"

- title: Student Travel Scholarship & Volunteer
  assoc: AAAI-26
  desc: Selected for a student travel scholarship and volunteer role at AAAI-26.
  date: "2026.01"

- title: Best Poster Award
  assoc: USC ECE 15th Annual Research Festival
  desc: Awarded among 110 participating teams.
  date: "2025.10"

- title: Daesang Foundation Scholarship
  assoc: Sogang University
  desc: Merit-based scholarship awarded from 2019 to 2023.
  date: "2019-2023"
```

Remove:

- Old `MS Honors Fellow @ University of Southern California / 2024`
- `Magna Cum Laude`
- `3rd Prize`

## 9. Education

Target file: `_data/edu.yml`

Replace with:

```yaml
- school: Texas A&M University
  degree: Ph.D.
  dept: Computer Science
  period: Aug. 2026 -

- school: University of Southern California
  degree: M.S.
  dept: Electrical Engineering, MS Honors Fellow
  period: Aug. 2024 - May. 2026

- school: Sogang University
  degree: B.S.
  dept: Electronic Engineering, Magna Cum Laude
  period: Mar. 2018 - Feb. 2024
```

Remove:

- `(Expected)` from USC
- `Micro-degree in Artificial Intelligence` from Sogang

## 10. Implementation Checklist For Later

- [x] Apply `_config.yml` sidebar changes.
- [x] Replace About prose and research paragraph.
- [x] Reorder homepage sections.
- [x] Add scrollable News container and CSS.
- [x] Add TAMU favicon assets and update head links.
- [x] Add Argonne logo asset and update work data.
- [x] Update publication venues and official URLs.
- [x] Update News entries.
- [x] Replace honors data.
- [x] Replace education data.
- [ ] Run static checks.
- [ ] Run GitHub Pages build or local Jekyll build if the Ruby environment is fixed.
- [ ] Push final batch after review.
