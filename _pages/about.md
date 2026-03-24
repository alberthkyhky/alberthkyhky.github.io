---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

Kang-Yang (Albert Huang) obtained his MSc degree in Computer Science at National Taiwan University, Taiwan, where he is part of the [AIMM](https://aimm.cmlab.csie.ntu.edu.tw/) group within the Communication and Multimedia Laboratory ([CMLab](https://www.cmlab.csie.ntu.edu.tw/new_cml_website/index.php)), under the guidance of [Prof. Wen-Huang Cheng](https://www.csie.ntu.edu.tw/~wenhuang/) and [Prof. Hong-Han Shuai](https://basiclab.lab.nycu.edu.tw/). Albert previously earned his B.S. degree from the Undergraduate Honors Program in Electrical Engineering and Computer Science at National Yang Ming Chiao Tung University, Taiwan. Additionally, he was an exchange student at RWTH Aachen University, Germany, from April to September in 2021. Albert's research interests are centered around the convergence of computer vision and deep learning. In the early stages of his academic journey, Albert specialized in lightweight deep learning, particularly in the areas of knowledge distillation and federated learning. Currently, Albert is broadening his research scope to include text-to-image generation and visual language models.

# 💻 Research Interests

- **Computer Vision:** image generation, image editing, video anomaly detection, interpretable DeepFake detection
- **Deep Learning:** federated learning, knowledge distillation, adversarial attack
  
<!-- === CV Download Module === -->
{% assign cv_path = "/files/Resume_Kang-Yang_Huang.pdf" %}
{% assign cv_file = site.static_files | where: "path", cv_path | first %}
<div class="cv-download">
  <a class="cv-btn" href="{{ cv_path | relative_url }}" target="_blank" rel="noopener" download>
    📄 Download My Academic CV
  </a>
  {% if cv_file %}
    <div class="cv-meta">
      <span>Last updated：{{ cv_file.modified_time | date: "%Y-%m-%d" }}</span>
    </div>
  {% endif %}
</div>

<style>
  .cv-download { margin: 12px 0 20px; }
  .cv-btn {
    display: inline-block;
    padding: 8px 14px;
    border-radius: 8px;
    background: #2b6cb0;
    color: #fff !important;
    text-decoration: none;
    font-weight: 500;
    transition: transform .06s ease-in-out, opacity .2s ease-in-out;
  }
  .cv-btn:hover { transform: translateY(-1px); opacity: .95; }
  .cv-meta {
    margin-top: 4px;
    font-size: 0.8em;
    color: #555;
  }
</style>

# 🔥 News

- _2026.03_: &nbsp;🎉🎉 We are organizing the 1st [TRIDENT: Tri-modal Deepfake Perception, Detection, and Hallucination Grand Challenge](https://tridentatmm26mgc.github.io/trident.github.io/) at ACM Multimedia, 2026 in Rio de Janeiro, Brazil.
- _2026.02_: &nbsp;🎉🎉 Our benchmark paper about tri-perspective DeepFake detection is accepted by CVPR 2026.
- _2025.07_: &nbsp;🎉🎉 Our research paper about face anti-spoofing utilizing vision-language model is accepted by ACM MM 2025.
- _2025.06_: &nbsp;🎉🎉 Received Hon Hai Technology Award, 2025 and Member of the Phi Tau Phi Scholastic Honor Society.
- _2025.01_: &nbsp;🎉🎉 Our survey paper about lightweight deep learning received the Best Paper Award for the year of 2024.
- _2024.11_: &nbsp;🎉🎉 Received Lam Research Outstanding Science Scholarship, 2024.
- _2024.07_: &nbsp;🎉🎉 Our research paper about image generation with precise human-object interactions through intelligent reasoning and correction is accepted by ACM MM 2024.
- _2024.06_: &nbsp;🎉🎉 Our research paper about weakly-supervised anomaly detection is accepted by IJCAI Workshop 2024.
- _2024.03_: &nbsp;🎉🎉 Our research paper about HOI detection is accepted for Oral by ICME 2024.
- _2022.06_: &nbsp;🎉🎉 Our survey paper about lightweight deep learning is accepted by IEEE Consumer Electronics Magazine.
- _2021.07_: &nbsp;🎉🎉 Our research paper about federated learning is accepted for Poster by ICME 2021.

# 📝 Publications
Please visit my [Google Scholar](https://scholar.google.com/citations?user=kd_B-7kAAAAJ&hl=en) page for full publications.

- <span class='paper-badge'>CVPR 2026</span> **TriDF: Evaluating Perception, Detection, and Hallucination for Interpretable DeepFake Detection**<br>
  _<u><b>Kang-Yang Huang*</b></u>, Ling Zou*, Jian-Yu Jiang-Lin*, Ling Lo, Sheng-Ping Yang, Yu-Wen Tseng, Kun-Hsiang Lin, Chia-Ling Chen, Yu-Ting Ta, Yan-Tsung Wang, Po-Ching Chen, Hongxia Xie, Hong-Han Shuai, Wen-Huang Cheng_<br>
  _IEEE/CVF Conference on Computer Vision and Pattern Recognition_, <b>CVPR</b>, 2026<br>
  <span class='paper-asset'><a href="https://j1anglin.github.io/TriDF/">Page</a></span> 
  <span class='paper-asset'><a href="https://arxiv.org/pdf/2512.10652">PDF</a></span> 
  <span class='paper-asset'><a href="https://j1anglin.github.io/TriDF/">Code</a></span>

- <span class='paper-badge'>ACM MM 2025</span> **InstructFLIP: Exploring Unified Vision-Language Model for Face Anti-spoofing**<br>
  _Kun-Hsiang Lin, Yu-Wen Tseng, <u><b>Kang-Yang Huang</b></u>, Jhih-Ciang Wu, Wen-Huang Cheng_<br>
  _ACM International Conference on Multimedia_, <b>ACM MM Oral</b>, 2025<br>
  <span class='paper-asset'><a href="https://kunkunlin1221.github.io/InstructFLIP/">Page</a></span> 
  <span class='paper-asset'><a href="https://dl.acm.org/doi/pdf/10.1145/3746027.3754939">PDF</a></span> 
  <span class='paper-asset'><a href="https://github.com/kunkunlin1221/InstructFLIP">Code</a></span>

- <span class='paper-badge'>ACM MM 2024</span> **ReCorD: Reasoning and Correcting Diffusion for HOI Generation**<br>
  _<u><b>Kang-Yang Huang*</b></u>, Jian-Yu Jiang-Lin*, Ling Lo, Yi-Ning Huang, Terence Lin, Jhih-Ciang Wu, Hong-Han Shuai, Wen-Huang Cheng_<br>
  _ACM International Conference on Multimedia_, <b>ACM MM Poster</b>, 2024<br>
  <span class='paper-asset'><a href="https://alberthkyhky.github.io/ReCorD/">Page</a></span> 
  <span class='paper-asset'><a href="https://dl.acm.org/doi/pdf/10.1145/3664647.3680936">PDF</a></span> 
  <span class='paper-asset'><a href="https://github.com/j1anglin/ReCorD">Code</a></span>

<!-- - <span class='paper-badge'>IJCAI W. 2024</span> **Dual Memory-guided Probabilistic Model for Weakly-supervised Anomaly Detection**<br>
  _Hsiu-Hua Chou, Ruyi Xu, <u><b>Kang-Yang Huang</b></u>, Jhih-Ciang Wu, Hong-Han Shuai, Wen-Huang Cheng_<br>
  _International Joint Conference on Artificial Intelligence Workshop_, <b>IJCAI W.</b>, 2024<br>
  <span class='paper-asset'><a href="https://link.springer.com/chapter/10.1007/978-981-97-9003-6_4">PDF</a></span>  -->

- <span class='paper-badge'>ICME 2024</span> **Learning Efficient Interaction Anchor for HOI Detection**<br>
  _Lirong Xue, <u><b>Kang-Yang Huang</b></u>, Rong Chao, Jhih-Ciang Wu, Hong-Han Shuai, Yung-Hui Li, Wen-Huang Cheng_<br>
  _IEEE International Conference on Multimedia and Expo_, <b>ICME Oral</b>, 2024<br>
  <span class='paper-asset'><a href="https://ieeexplore.ieee.org/document/10687459">PDF</a></span> 

- <span class='paper-badge'>IEEE MCE 2022</span> **Lightweight Deep Learning: An Overview**<br>
  _Ching-Hao Wang, <u><b>Kang-Yang Huang</b></u>, Yi Yao, Jun-Cheng Chen, Hong-Han Shuai, Wen-Huang Cheng_<br>
  _IEEE Consumer Electronics Magazine_, <b>IEEE MCE Best Paper Awards</b>, 2022<br>
  <span class='paper-asset'><a href="https://ieeexplore.ieee.org/document/9802879">PDF</a></span> 

- <span class='paper-badge'>ICME 2021</span> **Heterogeneous Federated Learning through Multi-branch Network**<br>
  _Ching-Hao Wang, <u><b>Kang-Yang Huang</b></u>, Jun-Cheng Chen, Hong-Han Shuai, Wen-Huang Cheng_<br>
  _IEEE International Conference on Multimedia and Expo_, <b>ICME Poster</b>, 2021<br>
  <span class='paper-asset'><a href="https://ieeexplore.ieee.org/document/9428189">PDF</a></span> 


# 💡 Projects

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">CVPR 2026</div><img src='images/CVPR26_TriDF.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

## [Multimodal Interpretable Deepfake Detection]()

  - <span class='paper-badge'>CVPR 2026</span> **TriDF: Evaluating Perception, Detection, and Hallucination for Interpretable DeepFake Detection**<br>
    _<u><b>Kang-Yang Huang*</b></u>, Ling Zou*, Jian-Yu Jiang-Lin*, Ling Lo, Sheng-Ping Yang, Yu-Wen Tseng, Kun-Hsiang Lin, Chia-Ling Chen, Yu-Ting Ta, Yan-Tsung Wang, Po-Ching Chen, Hongxia Xie, Hong-Han Shuai, Wen-Huang Cheng_<br>
    <span class='paper-asset'><a href="https://j1anglin.github.io/TriDF/">Page</a></span> 
    <span class='paper-asset'><a href="https://arxiv.org/pdf/2512.10652">PDF</a></span> 
    <span class='paper-asset'><a href="https://j1anglin.github.io/TriDF/">Code</a></span>

  - <span class='paper-badge'>ACM MM MGC 2026</span> **TRIDENT: Tri-modal Deepfake Perception, Detection, and Hallucination Grand Challenge**<br>
    <span class='paper-asset'><a href="https://tridentatmm26mgc.github.io/trident.github.io/">Page</a></span> 
    <span class='paper-asset'><a href="https://tridentatmm26mgc.github.io/trident.github.io/">Poster</a></span>

  - This project is supported by <span style="color:#76B900;">**NVIDIA**</span> Academic Grant Program.

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ACM MM 2025</div><img src='images/MM25_InstructFLIP.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

## [Vision-Language Model for Face Anti-spoofing](https://kunkunlin1221.github.io/InstructFLIP/)

- <span class='paper-badge'>ACM MM 2025</span> **InstructFLIP: Exploring Unified Vision-Language Model for Face Anti-spoofing**<br>
  _Kun-Hsiang Lin, Yu-Wen Tseng, <u><b>Kang-Yang Huang</b></u>, Jhih-Ciang Wu, Wen-Huang Cheng_<br>
 <b>Oral Presentation</b><br>
  <span class='paper-asset'><a href="https://kunkunlin1221.github.io/InstructFLIP/">Page</a></span> 
  <span class='paper-asset'><a href="https://dl.acm.org/doi/pdf/10.1145/3746027.3754939">PDF</a></span> 
  <span class='paper-asset'><a href="https://github.com/kunkunlin1221/InstructFLIP">Code</a></span>

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ACM MM 2024</div><img src='images/MM24_ReCorD.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

## [Diffusion for HOI Generation](https://alberthkyhky.github.io/ReCorD/)

- <span class='paper-badge'>ACM MM 2024</span> **ReCorD: Reasoning and Correcting Diffusion for HOI Generation**<br>
  _<u><b>Kang-Yang Huang*</b></u>, Jian-Yu Jiang-Lin*, Ling Lo, Yi-Ning Huang, Terence Lin, Jhih-Ciang Wu, Hong-Han Shuai, Wen-Huang Cheng_<br>
 <b>Poster Presentation</b><br>
  <span class='paper-asset'><a href="https://alberthkyhky.github.io/ReCorD/">Page</a></span> 
  <span class='paper-asset'><a href="https://dl.acm.org/doi/pdf/10.1145/3664647.3680936">PDF</a></span> 
  <span class='paper-asset'><a href="https://github.com/j1anglin/ReCorD">Code</a></span>

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">IJCAI W. 2024</div><img src='images/IJCAIW24_WAD.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

## [Diffusion for Industrial Anomaly Detection]()

- <span class='paper-badge'>IJCAI W. 2024</span> **Dual Memory-guided Probabilistic Model for Weakly-supervised Anomaly Detection**<br>
  _Hsiu-Hua Chou, Ruyi Xu, <u><b>Kang-Yang Huang</b></u>, Jhih-Ciang Wu, Hong-Han Shuai, Wen-Huang Cheng_<br>
  <b>Oral Presentation</b><br>
  <span class='paper-asset'><a href="https://link.springer.com/chapter/10.1007/978-981-97-9003-6_4">PDF</a></span>

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICME 2024</div><img src='images/ICME24_HOI.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

## [HOI Detection]()

- <span class='paper-badge'>ICME 2024</span> **Learning Efficient Interaction Anchor for HOI Detection**<br>
  _Lirong Xue, <u><b>Kang-Yang Huang</b></u>, Rong Chao, Jhih-Ciang Wu, Hong-Han Shuai, Yung-Hui Li, Wen-Huang Cheng_<br>
  <b>Oral Presentation</b><br>
  <span class='paper-asset'><a href="https://ieeexplore.ieee.org/document/10687459">PDF</a></span> 

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">IEEE MCE 2022</div><img src='images/MCE22_survey.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

## [Lightweight Deep Learning]()

- <span class='paper-badge'>IEEE MCE 2022</span> **Lightweight Deep Learning: An Overview**<br>
  _Ching-Hao Wang, <u><b>Kang-Yang Huang</b></u>, Yi Yao, Jun-Cheng Chen, Hong-Han Shuai, Wen-Huang Cheng_<br>
  <b>Best Paper Awards</b><br>
  <span class='paper-asset'><a href="https://ieeexplore.ieee.org/document/9802879">PDF</a></span> 

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICME 2021</div><img src='images/ICME21_mFedAvg.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

## [Federated Learning]()

- <span class='paper-badge'>ICME 2021</span> **Heterogeneous Federated Learning through Multi-branch Network**<br>
  _Ching-Hao Wang, <u><b>Kang-Yang Huang</b></u>, Jun-Cheng Chen, Hong-Han Shuai, Wen-Huang Cheng_<br>
  <b>Poster Presentation</b><br>
  <span class='paper-asset'><a href="https://ieeexplore.ieee.org/document/9428189">PDF</a></span> 

</div>
</div>

# 📖 Teaching

- Teaching Assistant, Computer Vision Practice with Deep Learning, National Taiwan University. (Spring 2023, Fall 2023)
- Teaching Assistant, Artificial Intelligence, National Taiwan University. (Spring 2024, Spring 2025)

# 📑 Academic Services

- Conference Reviewer: ACM MM'25, ICME'25, AAAI'26
<!-- - Journal Reviewer:  -->

# 🎖 Honors and Awards

- _2025.06_, Hon Hai Technology Award, 2025
- _2025.06_, Member of the Phi Tau Phi Scholastic Honor Society
- _2024.11_, Lam Research Paper Award, 2024

# 📫 References
### **Prof. Wen-Huang Cheng**
* **Title:** Professor, IEEE Fellow, CSIE Associate Chair
* **Department:** Department of Computer Science and Information Engineering
* **Institution:** National Taiwan University
* **Email:** `wenhuang@csie.ntu.edu.tw`
* **Role:** Academic Advisor for Graduate and Undergraduate Studies

---

### **Prof. Hong-Han Shuai**
* **Title:** Professor, Associate Chairman
* **Department:** Department of Electronics and Electrical Engineering
* **Institution:** National Yang Ming Chiao Tung University
* **Email:** `hhshuai@nycu.edu.tw`
* **Role:** Academic Advisor for Graduate and Undergraduate Studies

<div>