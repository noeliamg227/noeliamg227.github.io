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

Cloud computing is transforming healthcare by enabling remote monitoring, real-time data analysis, and improved collaboration between healthcare professionals. These advances are especially important for patients with chronic and progressive diseases such as **Amyotrophic Lateral Sclerosis (ALS)**.

ALS is a neurodegenerative disease that affects motor neurons, leading to progressive muscle weakness and loss of mobility. Because patients often require continuous monitoring, traditional hospital-based care can be challenging. Cloud-based systems provide an effective alternative.

---

## The Cloud-Based Solution
The system proposed by Corchiola et al. (2020), known as **SIMpLE DSS (Decision Support System)**, is a cloud-based platform designed to support:

- Remote patient monitoring  
- Teleconsultation  
- Storage and analysis of biomedical data  

It allows healthcare professionals to access patient data anytime and from anywhere.

---

## System Architecture
The platform integrates several components:

- **Web Server** → Manages user interaction and data processing  
- **Database Server** → Stores patient records and clinical history  
- **FTP Server** → Handles biosignal data (ECG, EMG, EEG)  
- **DICOM Server** → Stores and processes medical images (MRI, CT scans)  
- **Teleconsultation Module** → Enables communication between patients and doctors  

This architecture ensures a centralized and scalable system for managing healthcare data.

---

## Key Features
### Real-Time Monitoring
The system collects and visualizes physiological signals such as:
- ECG (heart activity)  
- EMG (muscle activity)  
- EEG (brain activity)  

Doctors can analyze these signals through web-based interfaces.

---

### Medical Imaging Support
The platform supports DICOM-standard images, allowing:
- Visualization of scans directly in the browser  
- Measurement of distances, angles, and areas  
- Collaborative analysis by multiple specialists  

---

### Telemedicine Integration
Patients and doctors can interact remotely through:
- Virtual consultations  
- Multi-user sessions  
- Continuous follow-up  

---

### Patient Data Management
Each patient has a complete digital profile including:
- Clinical history  
- Diagnostic tests  
- Sensor data  

The system also includes **data anonymization**, ensuring privacy and compliance with regulations.

---

## Advantages
{: .box-success}
**Key Benefits:**
- Improved access to healthcare from home  
- Continuous monitoring of patient conditions  
- Better collaboration between specialists  
- Scalable and flexible infrastructure  

---

## Challenges

{: .box-warning}
**Limitations to consider:**
- Data security and privacy concerns  
- Infrastructure and operational costs  
- Need for further clinical validation  

---

## Future Perspectives

Cloud-based systems like SIMpLE DSS represent the future of digital healthcare. Potential developments include:

- Integration with wearable devices  
- AI-driven diagnostics  
- Personalized treatment plans  

These technologies could significantly improve the quality of life for ALS patients and others with chronic diseases.

---

## Conclusion

Cloud computing is playing a crucial role in modern biomedicine. The SIMpLE DSS system demonstrates how cloud-based platforms can enable remote monitoring, enhance collaboration, and improve healthcare delivery for ALS patients.

As technology continues to evolve, cloud solutions will become increasingly central to patient care.

---

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

