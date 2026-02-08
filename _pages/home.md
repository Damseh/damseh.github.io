---
layout: home
title: Home
---

# Welcome to the Medical Image Computing Lab

We are a research group at the **United Arab Emirates University** led by **Dr. Rafat Damseh**, focusing on artificial intelligence and machine learning applications in healthcare and personalized medicine.

Our research spans medical image computing, computer-aided diagnostic systems, cerebrovascular network modeling, and biomedical data analysis using state-of-the-art deep learning techniques.

---

## Research Focus Areas

- **Medical Image Analysis**: Advanced segmentation, registration, and analysis of MRI, CT, and microscopy images
- **AI for Cancer Diagnostics**: Foundation models for precision oncopathology
- **Cerebrovascular Modeling**: Anatomical and biophysical modeling of brain vasculature
- **Computer-Aided Diagnostics**: Automated diagnostic and prognostic systems
- **Brain Connectivity**: Deep learning for structural connectivity analysis

---

## Latest News

{% assign sorted_news = site.data.news | sort: 'date' | reverse %}
{% for item in sorted_news limit:5 %}
**{{ item.date }}** - {{ item.title }}
{% if item.content %}
{{ item.content }}
{% endif %}

{% endfor %}

[See all news →](/news/)

---

## Featured Publications

See our [Publications page](/publications/) for the complete list.

- **2025**: New paper in *Artificial Intelligence in Medicine* on AI for pediatric medulloblastoma detection
- **2025**: Research on OCT-TPM vascular translation in *Scientific Reports*
- **2024**: Multiple papers in *Journal of Medical Internet Research* and *Scientific Reports*
- **2021**: Laplacian flow dynamics published in *IEEE Transactions on Medical Imaging*

---

## Open Source Software

We develop and maintain several open-source tools for biomedical imaging:

- **[VascGraph](https://github.com/Damseh/VascularGraph)**: Vascular network segmentation and analysis
- **[VirtualMRI](https://github.com/Damseh/virtualMRI)**: MRI response simulation framework
- **[AngioPulse](https://github.com/Damseh/angiopulse)**: Pulsatile flow dynamics in cerebral networks

---

## Join Our Team

We are always looking for motivated students (PhD, Master's, and undergraduate) interested in medical AI and machine learning. If you're passionate about applying AI to healthcare challenges, [contact us](/contact/)!

**Current Openings:**
- PhD positions in medical image analysis
- Master's thesis projects in deep learning for healthcare
- Undergraduate research assistants
