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
This post explores a real cloud-based biomedical system designed for remote monitoring of patients with Amyotrophic Lateral Sclerosis (ALS), based on Corchiola et al. (2020).

## Introduction

Amyotrophic Lateral Sclerosis (ALS) is a progressive neurodegenerative disease that affects motor neurons in the brain and spinal cord. As the disease advances, patients experience muscle weakness, atrophy, and severe mobility limitations.

Regular monitoring is essential, but frequent hospital visits can be difficult or even risky. This is where telemedicine and cloud computing provide a powerful alternative.


## The Proposed System: SIMpLE DSS
The proposed system, called **SIMpLE DSS (Decision Support System)**, is part of the SIMpLE project (Smart solutions for health Monitoring and independent mobiLity for Elderly and disabled people). It aims to improve the quality of life of patients with severe disabilities by enabling:

- Remote monitoring of physiological signals  
- Cloud-based storage of clinical data  
- Teleconsultation between patients and healthcare professionals  

The system integrates two main modules:

### 1. Biosignal Monitoring

The platform collects and analyzes key physiological signals such as:

- Electromyography (EMG)  
- Electrocardiography (ECG)  
- Electroencephalography (EEG)  

These signals are uploaded to the cloud and visualized through a web interface, allowing:

- Real-time and historical analysis  
- Signal comparison and overlap  
- Zooming and measurement of signal features  

---

### 2. Cloud-Based Data and Imaging Platform

The second module manages:

- Patient clinical records  
- Diagnostic imaging (DICOM standard)  
- Teleconsultation sessions  

Doctors can analyze medical images (CT, MRI, ultrasound) directly in the browser and perform:

- Length and area measurements  
- Angle calculations (e.g., Cobb angles)  
- Analysis of irregular regions  


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

Corchiola, D., Palumbo, A., Calabrese, B., Ielpo, N., Demeco, A., & Ammendolia, A. (2020). *Cloud-based biomedical system for remote monitoring of ALS patients*. IEEE International Conference on Bioinformatics and Biomedicine (BIBM).



[This is a link to a different site](https://deanattali.com/) and [this is a link to a section inside this page](#local-urls).

Here's a table:

| Number | Next number | Previous number |
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |

You can use [MathJax](https://www.mathjax.org/) to write LaTeX expressions. For example:
When \\(a \ne 0\\), there are two solutions to \\(ax^2 + bx + c = 0\\) and they are $$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

How about a yummy crepe?

![Crepe](https://beautifuljekyll.com/assets/img/crepe.jpg)

It can also be centered!

![Crepe](https://beautifuljekyll.com/assets/img/crepe.jpg){: .mx-auto.d-block :}

Here's a code chunk:

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

And here is the same code with syntax highlighting:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

And here is the same code yet again but with line numbers:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.

## Local URLs in project sites {#local-urls}

When hosting a *project site* on GitHub Pages (for example, `https://USERNAME.github.io/MyProject`), URLs that begin with `/` and refer to local files may not work correctly due to how the root URL (`/`) is interpreted by GitHub Pages. You can read more about it [in the FAQ](https://beautifuljekyll.com/faq/#links-in-project-page). To demonstrate the issue, the following local image will be broken **if your site is a project site:**

![Crepe](/assets/img/crepe.jpg)

If the above image is broken, then you'll need to follow the instructions [in the FAQ](https://beautifuljekyll.com/faq/#links-in-project-page). Here is proof that it can be fixed:

![Crepe]({{ '/assets/img/crepe.jpg' | relative_url }})

