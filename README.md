# DAC: Data Aggregation with Clustering

Code to reproduce Data Aggregation with Clustering as presented in the publication [DAC](https://)


## Install the dependencies
```
pip install -r requirements.txt
```

## Structure of the repository:

Simulation: apply DAC on a generated dataset
Real_Data: apply DAC on your own dataset

## DAC mechanism:

In demand forecasting one faces a tradeoff between using one model for each item (Decentralized approach) which corresponds to a high variance but a low bias or using one model 
for all items which gives access to more data for the model to train bubt potentially increases bias (Centralized approach).

There have been attempts to find a compromise by clustering some items together: one model for each category of items (pants, tops, hats...). 

The DAC method is a clever way to do a more sophisticated clustering. Based on the linear regession the idea is to estimate the coefficients for each feature.From statistical tests, the DAC identifies if a feature should be evaluated at the department level (for all items), at the cluster lever (by cluster) or at the sku level (one by item). From there each of the coefficient of the final regression will be evaluated at their differnet level by aggrating the observations from each items based on the identified structure.

If the feature "price_of_item" is identified as a cluster level feature, all the items from each cluster will share the same coefficient in the final linear regression and the coefficient will be estimated from aggregated datasets of the items from each cluster.


