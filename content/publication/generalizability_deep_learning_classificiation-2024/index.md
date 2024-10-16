---
title: "Generalizability of Deep Learning Classification of Spinal Osteoporotic Compression Fractures on Radiographs Using an Adaptation of the Modified-2 Algorithm-Based Qualitative Criteria"
date: 2023-07-10
authors:
- Qifei Dong
- Gang Luo
- Nancy E. Lane
- Li-Yung Lui
- Lynn Marshall
- Sandra K. Johnston
- Howard Dabbous
- Michael O’Reilly
- Ken F. Linnau
- Jessica Perry
- admin
- Jonathan Renslo
- David R. Haynor
- Jeffrey G. Jarvik
- Nathan M. Cross

# author_notes:
# - ""

publication_types: ["2"]
abstract: "**Rationale and Objectives:** Spinal osteoporotic compression fractures (OCFs) can be an early biomarker for osteoporosis but are often subtle, incidental, and underreported. To ensure early diagnosis and treatment of osteoporosis, we aimed to build a deep learning vertebral body classifier for OCFs as a critical component of our future automated opportunistic screening tool.

<br><br>**Materials and Methods:** We retrospectively assembled a local dataset, including 1790 subjects and 15,050 vertebral bodies (thoracic and lumbar). Each vertebral body was annotated using an adaption of the modified-2 algorithm-based qualitative criteria. The Osteoporotic Fractures in Men (MrOS) Study dataset provided thoracic and lumbar spine radiographs of 5994 men from six clinical centers. Using both datasets, five deep learning algorithms were trained to classify each individual vertebral body of the spine radiographs. Classification performance was compared for these models using multiple metrics, including the area under the receiver operating characteristic curve (AUC-ROC), sensitivity, specificity, and positive predictive value (PPV).

<br><br>**Results:** Our best model, built with ensemble averaging, achieved an AUC-ROC of 0.948 and 0.936 on the local dataset’s test set and the MrOS dataset’s test set, respectively. After setting the cutoff threshold to prioritize PPV, this model achieved a sensitivity of 54.5% and 47.8%, a specificity of 99.7% and 99.6%, and a PPV of 89.8% and 94.8%.

<br><br>**Discussion:** Analyses on the population-level and of densely tested zip codes (which contained most of the data) were similar between original and synthetically derived datasets. Analyses of sparsely tested populations were less similar and had more data suppression.

<br><br>**Conclusion:** Our model achieved an AUC-ROC>0.90 on both datasets. This testing shows some generalizability to real-world clinical datasets and a suitable performance for a future opportunistic osteoporosis screening tool.

"
featured: true
publication: "*Academic Radiology*"
doi: "10.1016/j.acra.2023.04.023"
tags: ["machine learning", "artificial intelligence", "osteoporosis" ,"compression fracture", "MrOS", "classification", "ensemble model", "imaging analysis", "radiograph"]
---