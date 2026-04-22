---
layout: post
title: Cloud Monitoring for ALS Patients
subtitle: A cloud-based system for remote healthcare
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [biomedicine, cloud, telemedicine]
comments: true
mathjax: true
author: Noelia Muñoz
---

{: .box-success}
This post explores a real cloud-based biomedical system designed for remote monitoring of patients with Amyotrophic Lateral Sclerosis (ALS), based on Yang et al. (2020).

## Introduction

Amyotrophic Lateral Sclerosis (ALS) is a progressive neurodegenerative disease that affects motor neurons in the brain and spinal cord. As the disease advances, patients experience muscle weakness, atrophy, and severe mobility limitations.

Regular monitoring is essential, but frequent hospital visits can be difficult or even risky. This is where telemedicine and cloud computing provide a powerful alternative.


## The Proposed System: SIMpLE DSS
The proposed system, called **SIMpLE DSS (Decision Support System)**, is part of the SIMpLE project (Smart solutions for health Monitoring and independent mobiLity for Elderly and disabled people). It aims to improve the quality of life of patients with severe disabilities by enabling:

- Remote monitoring of physiological signals  
- Cloud-based storage of clinical data  
- Teleconsultation between patients and healthcare professionals  

<div style="display:flex; justify-content:center;">
  <div style="text-align:center;">
    <img src="/images/fig1.png" width="400">
    <div style="margin-top:10px;">
      Figure 1: SIMpLE DSS software web-based architecture.
    </div>
  </div>
</div>

<br>
The system integrates two main modules:

  
### 1. Biosignal Monitoring

The platform collects and analyzes physiological signals such as:

- Electromyography (EMG)  
- Electrocardiography (ECG)  
- Electroencephalography (EEG)  

These signals are uploaded to the cloud and visualized through a web interface, allowing:

- Real-time and historical analysis  
- Signal comparison and overlap  
- Zooming and measurement of signal features  

### 2. Cloud-Based Data and Imaging Platform

The second module manages:

- Patient clinical records  
- Diagnostic imaging (DICOM standard)  
- Teleconsultation sessions  

Doctors can analyze medical images (CT, MRI, ultrasound) directly in the browser and perform:

- Length and area measurements  
- Angle calculations (e.g., Cobb angles)  
- Analysis of irregular regions  

<figure>

  <div style="display:flex; gap:20px; justify-content:center; flex-wrap:wrap;">
    <img src="/images/webviewer.png" style="width:540px; max-width:100%;">
    <img src="/images/measurement2.png" style="width:300px; max-width:100%;">
  </div>

  <figcaption style="text-align:center; margin-top:10px;">
    Figure 2 & 3: (Left) Web viewer. (Right) Length measurement.
  </figcaption>

</figure>



## Architecture

The system is built on a cloud-based architecture composed of:

- **Web Server**: handles user interface and data processing  
- **FTP Server**: stores biosignal streams  
- **Database Server**: manages patient and clinical data  
- **DICOM Server**: stores and processes medical images  
- **Teleconsultation Module**: enables remote communication  

## Features and Functionalities

- **Role-based access control**: patients, doctors, technicians, administrators
- **Patient geolocation**: for epidemiological analysis  
- **Customizable clinical records**
- **Real-time and historical data analysis**
- **Multi-specialist collaboration**
- **Data anonymization for privacy protection**

One particularly powerful feature is the dashboard, which allows clinicians to filter and analyze patient data based on multiple criteria (e.g., pathology, assigned doctor, type of exam), enabling efficient decision-making.

<div style="text-align:center;">

  <img src="/images/dashboard.png" width="400">

  <div style="margin-top:10px;">
    Figure 4: Example dashboard visualization.
  </div>

</div>

## Teleconsultation and Collaboration
The system supports many-to-many teleconsultation, meaning multiple doctors can evaluate the same patient simultaneously, specialists can collaborate remotely on complex cases and patients can receive multidisciplinary care without leaving home. This is especially valuable for ALS patients, who often require coordinated care from neurologists, physiotherapists, and other specialists.

## Impact and Future Potential

This cloud-based system represents a significant step forward in digital health and personalized medicine. Its benefits include:

- Improved accessibility to specialized care
- Reduced need for hospital visits
- Continuous monitoring of disease progression
- Enhanced collaboration among healthcare professionals

Beyond ALS, the platform could be adapted for other chronic conditions requiring long-term monitoring, such as cardiovascular or neurodegenerative diseases.

## References

T. Yang and Y. Zhao, "Application of cloud computing in biomedicine big data analysis cloud computing in big data," 2017 International Conference on Algorithms, Methodology, Models and Applications in Emerging Technologies (ICAMMAET), Chennai, India, 2017, pp. 1-3, doi: 10.1109/ICAMMAET.2017.8186626.

