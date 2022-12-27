# <strong>Stock Prediction Analysis using Regression-Enhanced Random Forest (REFR)<strong>

This notebook aims to analyse the prediction abilities of the Regression-Enhanced Random Forest model by H Zhang, D Nettleton and Z Zhu 
<br>Paper: https://arxiv.org/pdf/1904.10416.pdf<br>
<br>
The model will be used to predict Pepsi Stock (PEP), and compared against technical analysis based trading (SMA crossover) and simple machine learning (LASSO Regression) to test its effectiveness in both pre and post-Covid environments
<br>
# <strong>Conclusion</strong>
<strong>Portfolio value (USD) after 2 months</strong><br> 
<br>
SMA Crossover (pre-Covid): 103935.74 <br>
SMA Crossover (post-Covid): 103008.72 <br>
<br>
REFR based trading (pre-Covid): 104234.17 <br>
REFR based trading (post-Covid): 101179.52 <br>
<br>
<strong>RMSE comparison</strong><br>
<br>
linear model (pre-Covid): 0.609 <br>
linear model (post-Covid): 1.154 <br>
<br>
REFR model (pre-Covid): 0.537 <br>
REFR model (post-Covid): 1.144 <br>
<br>
In both pre and post-Covid environments, the RERF model improved the accuracy of the purely models marginally. The high REFR shows that while a purely linear model is not suited for predicting PEP stock post-Covid, the REFR model is successful in improving the accuracy of the predictions marginally. <br>
The effectiveness of the REFR model in pre-Covid environments can be seen by comparing REFR based trading against SMA crossover, whithe  <br>
    
This project can be improved with multi-variable models to enhance accuracy by analysing more factors which affect the stock market in diffeent environments, and it will be interesting to test the effectiveness of REFR applied onto multi-variable models. Further tuning of the model parameters are also required, and can be performed to improve the accuracy of the REFR model <br>
<br>
References: Zhang, H., Nettleton, D., & Zhu, Z. (2019). Regression-enhanced random forests. arXiv preprint arXiv:1904.10416.
