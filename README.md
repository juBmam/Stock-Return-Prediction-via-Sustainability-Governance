# Stock-Return-Prediction-via-Sustainability-Governance

Daily return and sustainability/diversity governance data was taken for 43 companies over the course of 5 years, of which only 2 had governance data. Each of the the governance data ids could be grouped into Subthemes and in turn overarching Themes, forming simplifying levels or granularities of features for modeling. At each level, the features are not strongly correlated, and there are few outliers in the yearly returns and volatility data. 

By modeling both yearly forward returns and volatility from the governance data from the same year, we find that using a Gradient Boosting model for volatility data at the subtheme level has an R2 of 39%. The most important features were Subthemes Q, V, W, S, and P. Similar levels of success where the yearly returns were modeled using a Gradient Boosting model reached an R2 of 36% at the theme level. However the interpretability of the two overarching themes masks the changes of the governance ids, forcing our hand to investigate a finer granularity.

Using an XGBoost model for forward returns, subthemes V, W, S, Q, and X were found to be the most important towards modeling the forward returns, albeit with a low R2 value of 0.03.
