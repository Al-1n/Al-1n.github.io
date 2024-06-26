---
layout: post
title: Optimizing GB Models for Medical Diagnosis
description: Evaluating Hyperopt, Optuna, and TunedThresholdClassifierCV 
img: /img/GB_Tuning_Thumb.png
---

**About the project**

![](/img/python_icon.png) ![](/img/jupyter_icon.png)

This project compared the performance of three gradient boosting algorithms (XGBoost, LightGBM, and CatBoost) on a binary classification task for medical diagnosis. The main focus was on improving prediction performance through hyperparameter and threshold optimization.

---

`Link to the project files:` <a href="https://github.com/Al-1n/Gradient_Boosting_Tuning">github.com/Al-1n/Gradient_Boosting_Tuning</a> 

`Full scientific report:`  <a href="https://github.com/Al-1n/Gradient_Boosting_Tuning/blob/main/Docs/GBT_classification_report.pdf">GBT Classification Report</a>

**Requirements**

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">Optuna</th>
    <th class="tg-0pky">Hyperopt</th>
    <th class="tg-0pky">LightGBM</th> 
    <th class="tg-0pky">CatBoost</th>    
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">XGBoost</td>
    <td class="tg-0pky">IpyWidgets</td>
    <td class="tg-0pky">Imblearn</td> 
    <th class="tg-0pky">Networkx</th>    
  </tr>
  <tr>
    <th class="tg-0pky">CloudPickle</th> 
    <td class="tg-0pky">Plotly</td>
    <td class="tg-0pky">SQLAlchemy</td>
    <td class="tg-0pky">ImageIO</td>    
  </tr>
  <tr>
    <th class="tg-0pky">PyWavelets</th> 
    <td class="tg-0pky">TiffFile</td>
    <td class="tg-0pky">Pandas</td>
    <td class="tg-0pky">Numpy</td>    
  </tr>
  <tr>
    <th class="tg-0pky">Seaborn</th> 
    <td class="tg-0pky">Matplotlib</td>
    <td class="tg-0pky">Math</td>
    <td class="tg-0pky">Sklearn</td>    
  </tr>
  <tr>
    <th class="tg-0pky">PyGraphViz</th> 
    <td class="tg-0pky">IPython</td>
    <td class="tg-0pky">JupyterLab</td>
    <td class="tg-0pky"></td>    
  </tr>
</tbody>
</table>
      
<br/>
**How to use this project**

The code in these files can be adapted to perform similar tests and comparisons for different datasets and models.  

Any environment that can load a python kernel and run jupyter notebooks such as *vs code*, *google collab* or *conda* can be used.


**Contributors**

<a href="https://www.linkedin.com/in/alin-airinei/">Alin Airinei</a>

---

<br/>    
# Data and Challenges
<br/>    
The analysis utilizes a popular sample of the Pima Indians Diabetes Database, which presents several challenges:
- Small sample size
- Numerous missing measurements 
- Class imbalance

To address these, the project employs model-based imputations, synthetic sampling for the minority class, and feature selection to refine the dataset.

# Methods
<br/>

**1. Data Preprocessing:**

- Model-based imputations using LightGBM
- Feature scaling
- ADASYN for data augmentation
- Feature selection with SelectKBest
- Class weighting

**2. Model Training and Optimization:**

- Baseline models without optimization
- Hyperparameter optimization using Optuna and Hyperopt
- Decision threshold optimization with TunedThresholdClassifierCV
 
# Performance Analysis
<br/>

**Recall Performance**

In medical diagnosis, recall (true positive rate) is crucial. Recall scores ranged from 0.64 to 0.89, with significant improvements observed through optimization.
  
- **XGBoost:** Highest recall achieved with Opt+Th optimization.
- **LightGBM:** Similar improvement pattern, with Opt+Th providing the best recall.
- **CatBoost:** Strong recall even at baseline, with Opt+Th yielding the highest recall.
 
 <p align="center" width="60%">
  <img src="/img/recall_bar_plot.png" alt=""><br/>
  <em>The grouped bar graph shows the recall performance of the three gradient boosting models (XGBoost, LightGBM, and CatBoost) across different optimization methods.
</em> 
</p>
<br/>   
 
**F1-Score Performance**

The F1-score balances precision and recall, critical for imbalanced datasets.

- **XGBoost:** Opt+Th optimization significantly improved the F1-score.
- **LightGBM:** Similar improvement with Opt+Th optimization yielding the highest F1-score.
- **CatBoost:** Strong baseline performance, with highest F1-score achieved through Opt+Th.

<p align="center" width="60%">
  <img src="/img/f1_score_bar_plot.png" alt=""><br/>
  <em>The grouped bar graph shows the F1-score performance of the three gradient boosting models (XGBoost, LightGBM, and CatBoost) across different optimization methods. </em> 
</p>
<br/>   

**AUROC and AUPRC**
 
**AUROC (Area Under the Receiver Operating Characteristic Curve):**
  
- **XGBoost and LightGBM:** High AUROC scores (0.78 to 0.83), with Optuna, Opt+Th, and Hyp+Th optimizers achieving the best results.
- **CatBoost:** Highest AUROC scores, maintaining around 0.83 with optimizations.
 
 <p align="center" width="60%">
  <img src="/img/auroc_line_plot.png" alt=""><br/>
  <em>The line plot shows the AUROC variation across different optimization methods for the three gradient boosting models. </em> 
</p>
<br/>   
 
**AUPRC (Area Under the Precision-Recall Curve):**

- **XGBoost:** Scores improved to 0.62 with Optuna and Opt+Th optimizers.
- **LightGBM:** Highest scores achieved with Optuna and Opt+Th (0.62).
- **CatBoost:** Leading with an AUPRC of 0.65, even at baseline.

<p align="center" width="60%">
  <img src="/img/auprc_line_plot.png" alt=""><br/>
  <em>The line plot shows the AUPRC variation across different optimization methods for the three gradient boosting models.
 </em> 
</p>
<br/>   

# Conclusions
<br/>    

1. Optimization techniques generally improved model performance across all metrics.
2. CatBoost demonstrated strong performance even with baseline parameters.
3. XGBoost and LightGBM benefited most from optimization, showing the largest improvements.
4. For scenarios prioritizing recall, such as medical diagnosis, optimized XGBoost and LightGBM models performed best.
5. CatBoost consistently outperformed in AUROC and AUPRC, indicating superior overall performance.
  
# Future Work
<br/>      

Further testing is recommended to confirm these findings and explore their applicability to other datasets and domains.

<br/>  
