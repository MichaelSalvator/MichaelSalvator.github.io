---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

[Download a PDF version of my CV]({{ base_path }}/files/cv.pdf) <!-- TODO: upload your CV PDF to the files/ folder and keep the name cv.pdf -->

Education
======
* **MSc in Computer Technology (Electronic Information)**, Hainan Normal University, 2024 - 2027 (expected)
  * College of Artificial Intelligence
  * Research focus: mangrove monitoring and species classification, satellite-derived bathymetry, deep learning for remote sensing
  * Advisor: <!-- TODO: your supervisor -->
* **BSc in Computer Science and Technology**, Hainan Normal University, 2020 - 2024

Research interests
======
* Remote sensing monitoring and fine-grained species classification of mangroves
* Satellite-derived bathymetry in optically complex coastal waters
* Deep learning for remote sensing image interpretation and change detection
* Quantum machine learning for remote sensing and spectral classification

Research experience
======
* **Long-term reconstruction and dynamic monitoring of mangrove habitat trajectories** (master's thesis)
  * 2025 - present, Hainan Normal University
  * Built a frequency-domain refinement adversarial network (Camelot-Net) that suppresses tidal, cloud-shadow and phenological noise in multi-year time series and removes spurious change points from per-pixel trajectories.
  * Introduced spatial-texture constraints along the time axis to fix the fragmentation in space and the abrupt jumps in time produced by pixel-level methods.

* **Fine-grained mangrove species classification with a hybrid quantum-classical neural network** (master's thesis)
  * 2025 - present, Hainan Normal University
  * Designed a hybrid quantum-classical network coupling red-edge feature enhancement with a variational quantum circuit to separate spectrally similar mangrove species.
  * Implemented quantum state encoding and variational quantum classifiers in Qiskit and QPanda, trained jointly with a classical convolutional feature extractor.

* **Lightweight shrimp segmentation and edge computing for complex aquaculture environments**
  * Oct 2025 - Oct 2026, National Innovation and Entrepreneurship Education Practice Base, Hainan Normal University
  * Project leader. Built a shrimp segmentation dataset of more than 8,000 images covering day, overcast and night conditions and clear versus turbid water.
  * Designed a lightweight MobileViTv3 network with multi-scale dilated convolutions and ECA channel attention; after structured pruning and quantisation it runs above 20 FPS and below 15 W on a Jetson edge device.

* **Satellite-derived bathymetry with Sentinel-2 and a Transformer model**
  * 2024 - 2026, Hainan Normal University
  * First author. Developed a Transformer-based retrieval model for Sentinel-2 multispectral data and validated it in optically complex coastal waters.

* **Remote sensing estimation of rubber plantation above-ground biomass and phenology**
  * 2025, 2025 Science and Technology Project, Hainan State Farms Investment Holding Group
  * Built a 170-dimensional feature set from Sentinel-2 imagery and 64 field plots, combining spectral bands, vegetation indices and GLCM texture; introduced an NDTI texture index with PCA.

* **Spatio-temporal accounting of mangrove blue carbon and future climate scenario simulation**
  * 2025, National Natural Science Foundation of China proposal (co-writer)
  * Helped design the four-stage roadmap: long-term dynamic mapping, multimodal AI blue-carbon accounting, spatio-temporal carbon accounting and future climate scenario simulation.

* **Key technologies for monitoring and assessing mangrove blue carbon with multi-source remote sensing**
  * 2025, Hainan Provincial Natural Science Foundation key project (contributor)
  * Contributed to the project rationale and literature review, and proposed a change detection network based on CNN and Transformer residual feature extraction.

* **Integrated communication, navigation and remote sensing equipment for marine fishery applications**
  * 2025, space-air-ground-sea programme feasibility study (co-writer)
  * Co-wrote the feasibility study report, reviewing fishery resource monitoring, vessel supervision and smart aquaculture early warning.

* **National Undergraduate Innovation and Entrepreneurship Training Program**
  * 2022, project leader, national-level project (completed)

* **Quantum Computing and Programming course projects**
  * 2025, independent work
  * Near-Earth object classification with a quantum naive Bayes classifier compared against a classical Gaussian naive Bayes model.
  * Classical KMeans compared with fidelity-based quantum KMeans in clustering quality, convergence and computational cost.

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% if post.category != 'under-review' %}
    {% include archive-single-cv.html %}
    {% endif %}
  {% endfor %}</ul>

Manuscripts under review
======
  <ul>{% for post in site.publications reversed %}
    {% if post.category == 'under-review' %}
    {% include archive-single-cv.html %}
    {% endif %}
  {% endfor %}</ul>

Talks and conferences
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>

Patents and software copyrights
======
* Time-series change detection of mangroves based on a multi-scale residual GRU network. Invention patent, 2026 (third inventor).
* Water depth inversion method based on particle swarm optimization and dynamic segmented ensemble learning. Invention patent, 2025 (fourth inventor).
* Body temperature detection and trajectory tracking method based on face recognition. Invention patent, 2022 (fifth inventor).
* Machine-learning-based epidemic prevention and detection system for local areas. Software copyright, 2021 (fifth contributor).

Code and data
======
* [MFSET](https://github.com/MichaelSalvator/MFSET) - mangrove pixel-level classification framework (spectral feature engineering, multi-model training, inference and spatial post-processing)
* [HESPERIA](https://github.com/MichaelSalvator/HESPERIA) - PyTorch implementation of reinforcement-learning-optimised masking policies for masked autoencoder pretraining on hyperspectral imagery
* [MRMS-GRU](https://github.com/MichaelSalvator/MRMS-GRU) - pixel-level mangrove change detection combining multi-scale 1D CNN with a bidirectional GRU

Honors and awards
======
* National Undergraduate Innovation and Entrepreneurship Training Program - national-level project, leader (2022)
* The 15th Chinese Collegiate Computing Competition - provincial first prize (2022)
* "Jiuqi Nuwa Cup" Hainan Provincial Low-Code Programming Competition - provincial first prize (2023)
* The 7th China International "Internet+" College Students' Innovation and Entrepreneurship Competition - university first prize (2021)
* The 14th "Higher Education Press Cup" National College Mathematical Contest in Modeling - provincial second prize (2023)
* Academic Scholarship, College of Artificial Intelligence, Hainan Normal University - second class (2026)
* Academic Scholarship, College of Information Science and Technology, Hainan Normal University (2023)

Skills
======
* **Programming and tools**: Python (PyTorch, TensorFlow, OpenCV, scikit-learn), ENVI, ArcGIS / QGIS, Google Earth Engine, Qiskit / QPanda, Git, Linux and GPU training environments
* **Remote sensing**: acquisition, preprocessing and atmospheric correction of Sentinel-1/2, Landsat, ICESat-2 / GEDI, hyperspectral and UAV imagery; feature engineering, model development and accuracy assessment
* **Languages**: Chinese (native), English (IELTS 6.5, August 2026)
