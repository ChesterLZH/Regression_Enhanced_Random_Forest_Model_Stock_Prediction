# <strong>Stock Prediction Analysis using Regression-Enhanced Random Forest (REFR)<strong>

This notebook aims to analyse the prediction abilities of the Regression-Enhanced Random Forest model by H Zhang, D Nettleton and Z Zhu <br>
Paper: https://arxiv.org/pdf/1904.10416.pdf<br>
<br>
# <strong>Approach</strong><br>
1. Pepsi Stock price data optained by calling API (source: AlphaVantage)
2. Exploratory Data Analysis and cleaning of data
3. Time series data split in pre and post-Covid periods
4. Time series data shifted to predict open prices using previous day data
4. LASSO Linear model built
5. REFR model built
6. Predicitons made using LASSO model and REFR model
<br>
# <strong>Metric<strong> <br>
1. RMSE used to compare effectiveness of ML models
2. Return on Investment of trades made using REFR predictions and SMA crossover were compared over a period of 2 months to determine model effectiveness
<br>
# <strong>Conclusion</strong><br>
In both pre and post-Covid environments, the RERF model improved the accuracy of the purely linear models marginally. The high REFR shows that while a purely linear model is not suited for predicting PEP stock post-Covid, the REFR model is successful in improving the accuracy of the predictions marginally. <br>
The effectiveness of the REFR model in pre-Covid environments can be seen by comparing REFR based trading against SMA crossover. <br>
<br>
Portfolio value (USD) after 2 months<br> 
- SMA Crossover (pre-Covid): 103935.74 <br>
- SMA Crossover (post-Covid): 103008.72 <br>
<br>
- REFR based trading (pre-Covid): 104234.97 <br>
- REFR based trading (post-Covid): 101179.52 <br>
<br>
RMSE comparison<br>
- linear model (pre-Covid): 0.609 <br>
- linear model (post-Covid): 1.154 <br>
<br>
- REFR model (pre-Covid): 0.532 <br>
- REFR model (post-Covid): 1.144 <br>
<br>
  
This project can be improved with multi-variable models to enhance accuracy by analysing more factors which affect the market environments, and it will be interesting to test the effectiveness of REFR applied onto multi-variable models. Further tuning of the model parameters are also required, and can be performed to improve the accuracy of the REFR model <br>
<br>
#References<br>
Zhang, H., Nettleton, D., & Zhu, Z. (2019). Regression-enhanced random forests. arXiv preprint arXiv:1904.10416.
