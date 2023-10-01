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

`Link to the project files:` <a href="https://github.com/Al-1n/IBM_SpaceX_Capstone/tree/master">SpaceX Launch Records</a> 

`Full report:`   [![](/img/spacex5.png)](https://github.com/Al-1n/IBM_SpaceX_Capstone/blob/master/SpaceX_Capstone_Project_Final_Report.pdf) 

---

The project workflow and most of the code in the project notebooks were authored by <a href="https://www.linkedin.com/in/joseph-s-50398b136/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDS0321ENSkillsNetwork26802033-2021-01-01">Joseph Santarcangelo</a>, <a href="https://www.linkedin.com/in/yan-luo-96288783/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDS0321ENSkillsNetwork26802033-2021-01-01">Yan Luo</a>, <a href="https://www.linkedin.com/in/nayefaboutayoun/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDS0321ENSkillsNetwork26802033-2021-01-01">Nayef Abou Tayoun</a>, and Lakshmi Holla for the IBM Data Science Certification Capstone Project. 

The project was organized into labs, with each lab corresponding to a step in a typical data science project lifecycle. The program participant was responsible for completing tasks, conducting analysis, and writing the final report.

You can read my comprehensive 67-page project report, which combines both technical and non-technical styles to describe each project step and discuss numerous insights from the data analysis, by following this link: <a href="https://github.com/Al-1n/IBM_SpaceX_Capstone/blob/master/SpaceX_Capstone_Project_Final_Report.pdf">Full report</a>. 

<a href="https://www.linkedin.com/in/alin-airinei/">Alin Airinei</a>

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

<br/>

<div style='text-align: center;' class='img_row'>
    <img class='col two' src='{{ site.baseurl }}/img/IBM_Professional_Certificate.png' alt=''/>    
</div>
<br/><br/><br/>

