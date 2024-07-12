# ML-Powerlifting
**Authors**
- Ankushev Vladislav
- Makarov Sergei 
- Shvartser Grigory
---
### Dataset Description
1. Dataset – from [Kaggle](https://www.kaggle.com/datasets/open-powerlifting/powerlifting-database/code)
2. It is a snapshot of the OpenPowerlifting database as of January 2024
3. OpenPowerlifting is creating a public-domain archive of powerlifting history
4. To see description of each column - go to Kaggle, find Data Explorer tab, click on 'openpowerlifting.csv'

![image](https://github.com/vladank99/ML-Powerlifting/assets/95710420/ff93c802-52de-4ccd-8f8e-91c0516fae26)

---
### Problem statement    
   
Can we predict **Best DeadLift?**     

Based on:
- **other types of Lifts** – Squat & Bench.
- **personal characteristics** – Age & Bodyweight

---

### ML task
- **Target:** Best 3 Deadlift
- **Predictors:** Age, Sex, Bodyweight, Best 3 Squat, Best3Bench
- **Models:** OLS regression, PCA & OLS regression
- **Metrics:** MAE, RMSE, R^2, Adj. R^2
- **Evaluation:** Cross-validation, VIF-analysis
--- 
### How to run the code
1. Download 'openpowerlifting-2024-01-06-4.csv' file from Kaggle
2. Download sufficient libraries using requirements.txt in CLI: pip install -r requirements.txt
3. Run each cell
--- 
### Results 
**OLS regression:** (best model, no overfitting)
- MAE = 14.1
- MAE (med) = 11.2
- RMSE = 18.6
- R2^2 = 0.9

**OLS & PCA regression:**
- PCA = 3 components
- MAE = 16.3
- MAE (med) = 16.3
- RMSE = 21.2
- R2^2 = 0.9

**Polinomal &  Ridge Regression:**
- MAE = 13.9
- MAE (med) = 11.2
- RMSE = 18.4
- R2^2 = 0.9

**Random forest:**
- MAE = 14.2
- MAE (med) = 11.5
- RMSE = 18.4
- R2^2 = 0.9
  
---
### Recommendations
We observed **underfitting in data**  
Model should be more complex   
List below - potential columns to add from external sources:
- height
- hand grip
- level of testeron
- foot size
- num of purchased equipment 

---
### Different types of Lift
![image](https://github.com/vladank99/ML-Powerlifting/assets/95710420/97cf797c-8c2d-4ac6-a4b6-d9d7bde53e12)


