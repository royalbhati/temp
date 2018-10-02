---
layout: post
title: "Evaluation Metrics in Machine Learning!"
date: 2018-10-2 16:32:20 +0300
description: Eval Metrics # Add post description (optional)
img:  # Add image post (optional)
---

# Evaluation Metrics!

There are various machine learning evaluation metrics available and every metric performs differently.Lets look at the evaluation metrics for Classification and Regression.

## Metrics for Regression

-   Mean Absolute Error
-   Mean Square Error
- Root mean squared error
-  Mean Absolute Percentage Error

###  Mean Absolute Error

The **mean absolute error** (MAE) is the simplest regression error metric to understand. We subtract the predicted value from the actual value and take its average over all the values. 

![MAE](/assets/img/mae.jpg)

###  Mean Square Error

The **mean square error** (MAE) is the another simple regression error in which we basically square the result of the subtraction of the predicted value from the actual value and take its average over all the values. 

![MSE](/assets/img/mse.jpg)


### Root mean squared error

Another similar error metric  is the  **root mean squared error**  (RMSE). As the name suggests, it is the square root of the MSE. Because the MSE is squared, its units do not match that of the original output. Researchers will often use RMSE to convert the error metric back into similar units, making interpretation easier.

![RMSE](/assets/img/rmse.jpg)

You can delete the current file by clicking the **Remove** button in the file explorer. The file will be moved into the **Trash** folder and automatically deleted after 7 days of inactivity.

###  Mean Absolute Percentage Error

The  **mean absolute percentage error**  (MAPE) is the percentage equivalent of MAE. The equation looks just like that of MAE, but with adjustments to convert everything into percentages.

![MAPE](/assets/img/mape.jpg)


### Conclusion on Regression Metrics

MAE and MAPE  has a clear interpretation since percentages are easier for people to conceptualize. MAPE and MAE are robust to the effects of outliers thanks to the use of absolute value.

The effect of the square term in the MSE equation is most apparent with the presence of outliers in our data. While each residual in MAE contributes **proportionally** to the total error, the error grows **quadratically** in MSE. This ultimately means that outliers in our data will contribute to much higher total error in the MSE than they would the MAE.

This is to say that large differences between actual and predicted are punished more in **MSE** than in **MAE**.

