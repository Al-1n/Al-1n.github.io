---
layout: post
title: Compton
description: Compton Scattering of gamma ray photons from low and high density metals
img: /img/CGRO_thumb.jpg

---

**About the project**

![](/img/python_icon.png) ![](/img/jupyter_icon.png)

This repository contains code for the analysis of data from an actual quantum mechanics experiment. The experiment utilized a monoenergetic gamma-ray source (Cs-137) and a photomultiplier detector to investigate the angle-dependent energy shift of scattered photons. This investigation provides a practical approach to determining the rest mass of the electron experimentally.

---
`Link to the project files:` <a href="https://github.com/Al-1n/Compton">github.com/Al-1n/Compton</a> 

`Full scientific report:`  <a href="https://github.com/Al-1n/Compton/blob/main/Compton_Paper.pdf">Angular Dependence of gamma rays scattered from a metal target (Compton Scattering)</a>

**Requirements**
* JupyterLab
* Pandas
* NumPy
* Lmfit
* Matplotlib

**How to use this project**

The code in these files can be adapted and used as a reference for analyzing data from scattering experiments. 

Any environment that can load a python kernel and run jupyter notebooks such as *vs code*, *google collab* or *conda* can be used.

In order to adapt the code to new measurements, a basic understanding on how to place, load and transform the data is required. 

**Contributors**

The experiment was performed under the guidance of Dr. Clark McGrew.

The data was collected at Stony Brook University by Nikhil Kumar, Xueqi Li, Edwin Ramillo and Makoto Tsuneto.

Data analysis performed by <a href="https://www.linkedin.com/in/alin-airinei/">Alin Airinei</a>. 

---
<br/>
# Background

<br/>
Compton's experiment marked a revolutionary turning point in the understanding of physics, as it not only confirmed Albert Einstein's 1905 proposal of energy quantization but also provided compelling evidence for the particle nature of light.

<br/>

<div style='text-align: center;' class='img_row'>
    <img class='col two' src='{{ site.baseurl }}/img/Time_Cover_Arthur_H_Compton.jpg' alt=''/>    
</div>
<div class='col two caption'>
    Arthur H. Compton 
</div>

<br/>  

In his seminal 1923 paper on the quantum theory of light scattering, A.H. Compton challenged the classical Thomson model of wave-matter interaction. He argued that the observed wavelength shift, resulting from the scattering of energetic X-rays or gamma rays by weakly bound electrons, could be better explained by considering a particle-like interaction between the incident 'radiation quantum' and the electron. This interaction caused the electron to recoil, leading to a frequency shift that resulted in the emission of a lower-energy photon. The energy difference was transferred to the electron, showcasing the dual nature of light as both waves and particles.

For his groundbreaking work, Arthur H. Compton was awarded the Nobel Prize in 1927 for his contributions to the understanding of X-rays. Later in his career, Compton played a pivotal role in the development of the Manhattan Project, a top-secret research and development project during World War II that led to the creation of the atomic bomb.

<br/>

<div style='text-align: center;' class='img_row'>
    <img class='col two' src='{{ site.baseurl }}/img/Alvarez_and_Compton.jpeg' alt=''/>    
</div>
<div class='col one caption'>
    Arthur H. Compton and his doctoral student, Luis Walter Alvarez, in 1933. Decades later, Alvarez and his son would become prominent advocates of the asteroid impact hypothesis, proposing that it was an asteroid impact that led to the extinction of the dinosaurs.Currently, the Alvarez hypothesis has been confirmed and is the mainstream theory of the K-Pg extinction event. 
</div>

<br/>   

# Results

<br/>

The results align with the particle theory of light, demonstrating that the energy difference between the scattered and incident rays is directly proportional to the energy of the electron. A comparison of these findings with the Compton model reveals a rest mass value for the electron that reasonably agrees with the accepted value.

For more information read the full report by following the link: <a href="https://github.com/Al-1n/Compton/blob/main/Compton_Paper.pdf">The Angular Dependence of Compton Scattering Cross-section Ratios of Cu and Al</a>. 

<a href="https://www.linkedin.com/in/alin-airinei/">Alin Airinei</a>

<br/>

<div style='text-align: center;' class='img_row'>
    <img class='col two' src='{{ site.baseurl }}/img/Cs_137.png' alt=''/>    
</div>
<div class='col one caption'>
    Uncalibrated Cs-137 spectrum, showing the leading 
Ba X-ray peak, the Pb X-ray, backscatter, Compton edge,
and the photopeak at 661.657 keV. 
</div>

<br/><br/><br/>
