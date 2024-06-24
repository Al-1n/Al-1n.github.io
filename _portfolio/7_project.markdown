---
layout: post
title: Optimizing GB Models for Medical Diagnosis
description: Evaluating Hyperopt, Optuna, and TunedThresholdClassifierCV on Gradient Boosting 
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
    <th class="tg-0pky">optuna</th>
    <th class="tg-0pky">hyperopt</th>
    <th class="tg-0pky">lightgbm</th> 
    <th class="tg-0pky">catboost</th>    
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">xgboost</td>
    <td class="tg-0pky">ipywidgets</td>
    <td class="tg-0pky">imblearn</td> 
    <th class="tg-0pky">networkx</th>    
  </tr>
  <tr>
    <th class="tg-0pky">cloudpickle</th> 
    <td class="tg-0pky">plotly</td>
    <td class="tg-0pky">sqlalchemy</td>
    <td class="tg-0pky">imageio</td>    
  </tr>
  <tr>
    <th class="tg-0pky">PyWavelets</th> 
    <td class="tg-0pky">tifffile</td>
    <td class="tg-0pky">pandas</td>
    <td class="tg-0pky">numpy</td>    
  </tr>
  <tr>
    <th class="tg-0pky">seaborn</th> 
    <td class="tg-0pky">matplotlib</td>
    <td class="tg-0pky">math</td>
    <td class="tg-0pky">sklearn</td>    
  </tr>
  <tr>
    <th class="tg-0pky">pygraphviz</th> 
    <td class="tg-0pky">IPython</td>
    <td class="tg-0pky"></td>
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

<br/>   
- Model-based imputations using LightGBM
- Feature scaling
- ADASYN for data augmentation
- Feature selection with SelectKBest
- Class weighting

**2. Model Training and Optimization:**
<br/>  
- Baseline models without optimization
- Hyperparameter optimization using Optuna and Hyperopt
- Decision threshold optimization with TunedThresholdClassifierCV
 
# Performance Analysis

<br/>  
**Recall Performance**

<br/>  
In medical diagnosis, recall (true positive rate) is crucial. Recall scores ranged from 0.64 to 0.89, with significant improvements observed through optimization.
  
- **XGBoost:** Highest recall achieved with Opt+Th optimization.
- **LightGBM:** Similar improvement pattern, with Opt+Th providing the best recall.
- **CatBoost:** Strong recall even at baseline, with Opt+Th yielding the highest recall.
 
**F1-Score Performance**

<br/>  
The F1-score balances precision and recall, critical for imbalanced datasets.

- **XGBoost:** Opt+Th optimization significantly improved the F1-score.
- **LightGBM:** Similar improvement with Opt+Th optimization yielding the highest F1-score.
- **CatBoost:** Strong baseline performance, with highest F1-score achieved through Opt+Th.

**AUROC and AUPRC**

<br/>  
**AUROC (Area Under the Receiver Operating Characteristic Curve):**

<br/>  
- **XGBoost and LightGBM:** High AUROC scores (0.78 to 0.83), with Optuna, Opt+Th, and Hyp+Th optimizers achieving the best results.
- **CatBoost:** Highest AUROC scores, maintaining around 0.83 with optimizations.
 
**AUPRC (Area Under the Precision-Recall Curve):**

<br/>  
- **XGBoost:** Scores improved to 0.62 with Optuna and Opt+Th optimizers.
- **LightGBM:** Highest scores achieved with Optuna and Opt+Th (0.62).
- **CatBoost:** Leading with an AUPRC of 0.65, even at baseline.

# Conclusions

<br/>   
1. Optimization techniques generally improved model performance across all metrics.
2. CatBoost demonstrated strong performance even with baseline parameters.
3. XGBoost and LightGBM benefited most from optimization, showing the largest improvements.
4. For scenarios prioritizing recall, such as medical diagnosis, optimized XGBoost and LightGBM models performed best.
5. CatBoost consistently outperformed in AUROC and AUPRC, indicating superior overall performance.

<br/>   
# Future Work

<br/>   
Further testing is recommended to confirm these findings and explore their applicability to other datasets and domains.

<br/>  
