---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a final-year PhD candidate in Machine Learning, jointly trained between ETIS Lab, CY Cergy Paris University / ENSEA / CNRS, France, and the Computer Vision Laboratory at the University of Ljubljana, Slovenia, through the [EUTOPIA](https://eutopia-university.eu/) co-tutelle programme.

I am supervised by [Prof. Dr. Peter Peer](https://scholar.google.fr/citations?&user=-h43hWoAAAAJ), [Prof. Dr. Vassilis Christophides](https://scholar.google.fr/citations?user=MdUjsa8AAAAJ&oi=sra), [Assoc. Prof. Dr. Vitomir Štruc](https://scholar.google.fr/citations?user=kr52cmAAAAAJ&oi=sra), and [Assoc. Prof. Dr. Son Vu](https://scholar.google.fr/citations?user=Fw14qXwAAAAJ&oi=ao).

My research focuses on generative AI robustness, synthetic-media detection, self-supervised and contrastive representation learning, model evaluation under distribution shift, and efficient neural architectures. I am especially interested in building evaluation pipelines and learning systems that remain reliable beyond narrow benchmark settings.

I have published work at CVPR, ICCV, and BMVC. My recent projects include SeeABLE, a contrastive learning framework for exposing deepfakes; QN-Mixer, an optimization-inspired neural architecture for sparse-view CT reconstruction; and SSD, a neural-collapse-inspired approach to contrastive continual learning.

I am currently interested in research scientist, research engineer, and machine learning roles involving AI safety evaluations, model robustness, multimodal systems, generative AI, quantitative machine learning, and reliable AI systems.

Before joining the PhD, I received an engineering degree from ENSEA, École nationale supérieure de l'électronique et de ses applications, with a specialization in Computer Science, Systems, Artificial Intelligence, and Big Data.

## News

- **2024:** QN-Mixer accepted at CVPR 2024.
- **2024:** SSD accepted at BMVC 2024.
- **2023:** SeeABLE accepted at ICCV 2023.

## Selected Projects

### Unified Deepfake Evaluation Framework

Private research framework for standardized deepfake evaluation across datasets. It manages dataset manifests, video frame extraction with ffmpeg, detector interfaces, PyTorch loaders, data augmentation, and frame/video-level metrics such as accuracy and AUROC.

### QN-Mixer

Project page for CVPR 2024 work on sparse-view CT reconstruction.  
[Project page](https://towzeur.github.io/QN-Mixer/)

### Gym Abalone

OpenAI Gym-style reinforcement learning environment for the board game Abalone.  
[GitHub](https://github.com/towzeur/gym-abalone)

## Publications

{% include base_path %}

{% assign sorted = site.publications | reverse %}
{% for post in sorted %}
  {% include archive-single.html %}
{% endfor %}