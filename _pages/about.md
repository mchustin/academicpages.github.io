---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

I am a first-year Ph.D. candidate at the **HKUST NLP Group**, Department of Computer Science and Engineering, Hong Kong University of Science and Technology (HKUST), where I am fortunate to be advised by [Prof. Junxian He](https://jxhe.github.io/). 

Prior to joining HKUST, I received my B.Eng. degree from **Shanghai Jiao Tong University (SJTU)** in June 2024. During my undergraduate studies at SJTU, I was honored to receive the **Zhiyuan Honor Scholarship** and began conducting research under the supervision of Prof. Junxian He.

Research Interests
======
My primary research interests lie broadly in **Natural Language Processing (NLP)** and **Machine Learning (ML)**. Currently, I am actively working on:
* **LLM Reasoning & Reinforcement Learning**: Developing methods to synthesize verifiable reasoning datasets at scale and exploring reinforcement learning algorithms to enhance logical reasoning in foundation models.
* **Hallucination in Vision-Language Models (VLMs)**: Investigating multimodal perception bottlenecks and fine-grained visual comprehension challenges to mitigate hallucinations in VLMs.
* **LLM Truthfulness & Interpretability**: Analyzing the internal geometry, representation dynamics, and universal truthfulness hyperplanes within large language models to improve reliability.

Experience & Research Internships
======
* **MINIMAX** (February 2025 – Present)  
  *Research Intern*  
  Focusing on frontier LLM reasoning, reinforcement learning, and alignment.

* **Tencent WXG** (June 2024 – September 2024)  
  *Research Intern* (Advisor: Zifei Shan)  
  Conducted research on Vision-Language Models and multimodal chart understanding.

* **Shanghai AI Lab** (June 2023 – December 2023)  
  *Research Intern* (Advisor: Prof. Yu Cheng)  
  Conducted research on LLM internal representation geometry and truthfulness.

Recent News & Updates
======
* **[2025]** Released preprint *"SynLogic: Synthesizing Verifiable Reasoning Data at Scale for Learning Logical Reasoning and Beyond"*.
* **[2025]** Released preprint *"On the Perception Bottleneck of VLMs for Chart Understanding"*, with code available at [Vision4Chart](https://github.com/Vicent0205).
* **[2024]** Paper *"On the Universal Truthfulness Hyperplane Inside LLMs"* accepted to **EMNLP 2024**! Code released at [Universal_Truthfulness_Hyperplane](https://github.com/Vicent0205).
* **[2024]** Co-authored paper *"In-Context Sharpness as Alerts: An Inner Representation Perspective for Hallucination Mitigation"* accepted to **ICML 2024**.
* **[2024]** Graduated with B.Eng. from Shanghai Jiao Tong University and commenced Ph.D. studies at HKUST.
* **[2023]** Co-authored papers *"C-Eval: A Multi-Level Multi-Discipline Chinese Evaluation Suite for Foundation Models"* and *"Composing Parameter-Efficient Modules with Arithmetic Operations"* accepted to **NeurIPS 2023**.

Publications
======
You can also view these on the dedicated [Publications page](/LJT-Homepage/publications/) or on my [Google Scholar profile](https://scholar.google.com/citations?hl=en&user=tbK9jl4AAAAJ&view_op=list_works&sortby=pubdate).

{% if site.publication_category %}
  {% for category in site.publication_category %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h3>{{ category[1].title }}</h3>
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}

Skills & Competencies
======
* **Research Domains**: Large Language Models (LLMs), Vision-Language Models (VLMs), Reasoning & Verification, Reinforcement Learning (RL), Model Truthfulness & Interpretability, Benchmark & Evaluation.
* **Programming & Frameworks**: Python, PyTorch, Hugging Face (Transformers, Datasets, Accelerate), DeepSpeed, vLLM, C/C++, Shell/Bash, Git, LaTeX.
* **Languages**: Chinese (Native), English (Fluent).

Contact
======
* **Email**: [jliugi@connect.ust.hk](mailto:jliugi@connect.ust.hk)
* **GitHub**: [@Vicent0205](https://github.com/Vicent0205)
* **Google Scholar**: [Junteng Liu's Profile](https://scholar.google.com/citations?hl=en&user=tbK9jl4AAAAJ&view_op=list_works&sortby=pubdate)
* **X (Twitter)**: [@junteng88716710](https://x.com/junteng88716710)
* **Address**: HKUST NLP Group, Department of Computer Science and Engineering, The Hong Kong University of Science and Technology, Clear Water Bay, Kowloon, Hong Kong
