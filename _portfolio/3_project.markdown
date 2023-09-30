---
layout: post
title: SpaceX Launch Records
description: Catching Up in the Space Race
img: /img/spacex1_thumb.jpg
---

**About the project**

![](/img/python_icon.png) ![](/img/jupyter_icon.png) ![](/img/folium_logo.png) ![](/img/plotly_icon.png)

In this project, we utilize Data Science tools to analyze and map the critical components that have defined SpaceX's successful business model, securing its leadership position in the space launch industry.

---

`Link to the project files:` <a href="https://github.com/Al-1n/DFFS">github.com/Al-1n/DFFS</a> 

`Full scientific report:`  <a href="https://github.com/Al-1n/DFFS/blob/main/SatSpec_Revision2_Scientific_Paper.pdf">Doppler Free Saturation Spectroscopy of Rubidium</a>

---

<br/>

# Background
<br/>  
In the rapidly expanding space industry, SpaceX, headquartered in Hawthorne, California, stands as a trailblazer. The company's Falcon 9 rockets are renowned for their punctual payload deliveries to orbit, made possible in part by the innovative reuse of their first-stage rockets. This not only ensures reliability but also substantially reduces the cost of launching payloads into space. SpaceX has even achieved a remarkable record of refurbishing and relaunching the same booster within a mere 27 days.

As the space economy continues to soar, with Bank of America projecting a staggering $2.7 trillion valuation by 2045, the pressure intensifies on competitors to keep up. However, development challenges and high expenses frequently plague rival companies, causing frustrating delays for customers with time-sensitive payload launch schedules. To address this dynamic landscape, numerous industry leaders, including Blue Origin and Boeing, are developing their own reusable launchers.

Using the tools of Data Science, this project aims to unravel key facets of SpaceX's business model, offering insights that potential competitors can leverage in their pursuit of challenging SpaceX's dominance in the industry.

<div style='text-align: center;' class='img_row'>
    <img class='col two' src='{{ site.baseurl }}/img/spacex2.jpg' alt=''/>
</div>
<div class='col two caption'>
    Image credit <a href='https://commons.wikimedia.org/wiki/User:Dnn87'>Dnn87</a>. This file is licensed under the <a href='https://en.wikipedia.org/wiki/en:Creative_Commons'>Creative Commons</a> <a href='https://creativecommons.org/licenses/by/3.0/deed.en'>Attribution 3.0 Unported</a> license.
</div>
<br/>  

### Some of the insights drawn from the analysis  
<br/>   
From the analysis of the flight density for each launch site it was established that the bulk of the
SpaceX missions are handled at Florida sites with the Cape Canaveral SLC-40 site at the lead followed
by the Kennedy Space Center.

Building on the above insight we looked at the payload range for each location and confirmed that
CCAFS SLC-40 and KSC LC-39A share similar payload ranges while the Vandenberg location on the West
coast does not handle payloads larger than 10000 Kg.

By comparing the success rates of different orbit types it became noticeable that launches following
a polar trajectory have a strikingly high rate of successful landings. Future investigations need to take a
more in dept look at the relation between polar trajectories and landing outcomes.

Looking at the frequency of each orbit type we observed that low Earth orbits are by far the bulk of
the business at the current time, with GTO missions at the higher altitude limit. We also observed a
shift in frequency between GTO and VLEO with the emergence of the B5 boosters.

By analyzing the payload mass range specific to each orbit we deduced that GTO has a well defined
range (between 3000 and 7000 Kg) while ISS has the widest range of payloads. The highest payloads,
corresponding to VLEO orbits might also be explained by the higher capacity of the latest boosters.

<br/>
### Summary of other insights
<br/>
(for a full discussion check the full report following the link above)
<br/>

* The yearly trend for Falcon 9 booster landing success shows improvement from 2013 to 2020 due to ongoing technology enhancements.

* SpaceX had four unique launch locations, with two referring to the same Cape Canaveral location.

* NASA was SpaceX's main customer during early test flights, emphasizing reusability as a goal.

* For early LEO missions, payloads were notably lighter than the rocket's specifications.

* Flight 20 marked the first true landing of a first-stage Falcon 9 booster.

<div style='text-align: center;' class='img_row'>
    <img class='col two' src='{{ site.baseurl }}/img/global_detail_Florida.png' alt=''/>    
</div>
<div class='col three caption'>
    Detail showing the Kennedy LC and Cape Canaveral SLC launch sites in Florida. 
</div>
<br/>       

### More insights...
<br/>
* Identifying booster names for specific payload ranges highlighted technological advancements in Falcon 9 rockets.

* SpaceX attempted to land only 70% of missions, warranting further investigation into factors influencing landing opportunities.

* Block 5 boosters offer the highest payload capacity.

* Drone ship landings were more frequent in early flights, possibly due to safety concerns.

* Proximity analysis underscored the importance of site location near the Equator for launch efficiency and proximity to large bodies of water for safety.

* Decision Tree models demonstrated the highest predictive accuracy among classification models, with future developments benefiting from new data.

<div style='text-align: center;' class='img_row'>
    <img class='col two' src='{{ site.baseurl }}/img/Confusion.png' alt=''/>    
</div>
<div class='col two caption'>
    Evaluation of the highest performing classification model. 
</div>


<br/><br/><br/>

