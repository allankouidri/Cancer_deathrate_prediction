# Multiple linear regression and descision tree

## Advanced statistic and machine learning

### Prediction of the cancer death rate.

This work uses data aggregated from a number of sources including the American Community Survey [census.gov](http://census.gov/), [clinicaltrials.gov](http://clinicaltrials.gov/), and [cancer.gov](http://cancer.gov/) 🏥. 
The dataset contains 3048 datapoints and 33 variables.

🚩 In this project we build and compared several models to predict the "TARGET_deathRate". We tested ordinary least square (OLS) regression, CART and Random Forest algorithms. We also used VSURF for variable selection.

Models were compared using the root mean squared error (RMSE): 


| **Model**                      | **RMSE** |
|--------------------------------|----------|
| OLS full dataset (numericals)  | 19.259   |
| OLS without outliers           | 15.174   |
| Step default parameters        | 15.173   |
| Step forward or backward       | 15.165   |
| LASSO                          | 15.248   |
| OLS on LASSO selected features | 15.254   |
| CART final tree                | 17.598   |
| CART + VSURF final tree        | 17.861   |
| Random Forest                  | 14.738   |


⚪ We condlude that the best model to predict "TARGET_deathRate"  is Random Forest followed by step method forward or backward.



