---
permalink: /
title: "academicpages is a ready-to-fork GitHub Pages template for academic personal websites"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a second year Deep Learning Ph.D. student at CY Cergy Paris, France University funded by [EUTOPIA](https://eutopia-university.eu/)
co-tutelle programme with the Ljubljana University, Slovenia.
I am supervised by Prof. [Prof. Dr. Peter Peer](https://scholar.google.fr/citations?&user=-h43hWoAAAAJ) & [Prof. Dr. Vassilis Christophides](https://scholar.google.fr/citations?user=MdUjsa8AAAAJ&oi=sra) with the
co-supervision of [Assoc. Prof. Dr. Vitomir Štruc](https://scholar.google.fr/citations?user=kr52cmAAAAAJ&oi=sra) & [Assoc. Prof. Dr. Son Vu](https://scholar.google.fr/citations?user=Fw14qXwAAAAJ&oi=ao).


I am mainly doing research on Deepfake detection.
My main goal is to improve the generalization of forgery detection methods to new datasets and new types of forgery.
I am interested in the application of self-supervised learning in the field of computer vision. 
Application wise, I hope that my research will help to improve forgery detection in the wild.

Before joining the Ph.D., I received my undergraduate degree in engineering from ENSEA, 
École nationale supérieure de l'électronique et de ses applications.

## News
- <span style="color:blue">[New preprint]:</span> We framed Forgery Detection as a One Class Out Of Distribution problem. We wrote a paper summarizing our findings.
Find the paper [soon](arxiv).


## Publications

{% include base_path %}

{% assign sorted = site.publications | reverse %}
{% for post in sorted %}
  {% include archive-single.html %}
{% endfor %}

