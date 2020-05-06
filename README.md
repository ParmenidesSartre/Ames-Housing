# Ames Housing Dataset

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ParmenidesSartre/Ames-Housing/master?urlpath=https%3A%2F%2Fgithub.com%2FParmenidesSartre%2FAmes-Housing%2Fblob%2Fmaster%2FNotebook.ipynb)

# Abstract
Ames Housing Dataset contained what a typical home buyer would want to know before making a purchase. In this analysis i will try answer question such as: 
  - What are the variables that have the most inﬂuences on the sales price ? 
  - Do Overall Quality of the house affects the sale price ? 
  - Do Sales Condition of the house affects the sale price ?
  
The relevant variables are plotted using box plot,scatter plot and bar chart to find connection between them. Some statistical test such as correlation and multicollinearity also have been done. We found out that variable such as age of the house and size of the house play a major part in driving up the sales price.

# Treatment of Outliers
![alt text](https://github.com/ParmenidesSartre/Ames-Housing/blob/master/Pictures/Outliers.png)

# Distribution of Sales Price
![alt text](https://github.com/ParmenidesSartre/Ames-Housing/blob/master/Pictures/Sale%20Price%20B.png)

# What affects House Price?
![alt text](https://github.com/ParmenidesSartre/Ames-Housing/blob/master/Pictures/Sale%20conds.png)

# Machine Learning Performance
![alt text](https://github.com/ParmenidesSartre/Ames-Housing/blob/master/Pictures/ML%20Curves.png)

# Conclusions 
What are the variables that have the most inﬂuences on the sales price ? 
  - Above ground living area square feet,size of garage and total square feet of basement area.

How is the sales price distributed ? 
  - The sale price doesn’t follow normal distribution. Fixed using natural log.
  
Does the variable shows multicollinearity ? 
  - Yep.
  
Do Overall Quality of the house affects the sale price ? 
  - Higher rating for overall quality increase the sale price.
  
Do Sales Condition of the house affects the sale price 
  - The price of normal house has more spread than any of the other type of sale condition. Sales within family on the other hand, shows     a small spread which makes sense because people tend to value their family more and decide to not charge exorbitant price. Partial       home which is new house has higher mean price value than other type of sales condition. Therefore, i do think sale condition has low     impact on the sales price except for new houses.

What is the best machine learning algorithm for this dataset. Ensemble or simple model such as Lasso and Elastic Net ? 
  - Elastic Net does the job just fine. Huge number of features makes linear models more powerful. The performance gain using ensemble       method is not worth it considering the computation resources required. Elastic Net managed to score 0.1094 on the training set while     scoring 0.1181 on the training set.
