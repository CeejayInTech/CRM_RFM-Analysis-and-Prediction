# CRM_RFM-Analysis-and-Prediction

###  CRM-RFM analysis is a customer segmentation technique that groups customers based on their Recency of a purchase, Frequency of purchases, and Monetary value of their spending. It is used within a Customer Relationship Management (CRM) system to create targeted marketing campaigns by identifying valuable customer segments and tailoring strategies to improve retention, sales, and customer loyalty.

#### The RFM model evaluates customers based on three key metrics:

*Recency:* How recently a customer has made a purchase

*Frequency:* How frequently a customer makes purchases

*Monetary Value:* How much a customer spends on purchases 

### Dataset: Kaggle

#### Segments

RFM analysis assigns each customer a score for each of these metrics, which are then used to segment customers into groups based on their overall score.

*Champions:* Bought recently, buy often and spend the most. 

*Loyal Customers:* Spend good money with us often. Responsive to promotions.

*Potential Loyalist:* Recent customers, but spent a good amount and bought more than once.

*New Customers:* Bought most recently, but not often.

*Promising:* Recent shoppers, but haven’t spent much.

*Need Attention:* Above average recency, frequency and monetary values. May not have bought very recently though.

*About To Sleep:* Below average recency, frequency and monetary values. Will lose them if not reactivated.

*At Risk:* Spent big money and purchased often. But a long time ago. Need to bring them back.

*Can’t Lose Them:* Made the biggest purchases, and often. But haven’t returned for a long time.

*Hibernating:* Last purchase was long back, low spenders and bought seldomly. 

*Lost:* Customers who have not made any purchase recently.

#### This segmentation helps businesses identify which customers are most valuable and should receive priority attention, and which customers are less valuable and may require less attention or targeted marketing efforts.

###  Model Evaluation Report

A linear regression model was developed to predict the target variable based on selected features. The model’s performance was assessed using key statistical metrics, including the coefficient of determination (R²), mean squared error (MSE), and mean absolute error (MAE).

| Metric  | Value          | Interpretation                                                                                                                                                                                                                                                                 |
| :------ | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **R²**  | **0.630**      | The model explains approximately **0.630% of the variance** in the target variable. This indicates a moderate level of predictive power — the model captures more than half of the underlying data patterns, but a significant portion of variability remains unexplained.      |
| **MSE** | **113,867.17** | The mean squared error suggests that the **average squared deviation** between predicted and actual values is relatively large. While MSE is sensitive to outliers, this result implies the presence of prediction errors that may be influenced by high-variance data points. |
| **MAE** | **253.23**     | On average, the model’s predictions deviate by **253.23 units** from the true values. Since MAE retains the same unit as the target variable, it reflects a **moderate error margin**, acceptable for preliminary analysis but improvable through feature optimization.         |


####  Prediction Interpretation

The model demonstrates a reasonable fit, suggesting that the predictors contribute meaningfully to the target outcome. However, the R² value also highlights that nearly half of the variation remains unexplained, which may point to:

Nonlinear relationships that linear regression cannot fully capture,

Omitted or weakly correlated predictors,

Potential multicollinearity among features, or

Measurement errors or noise in the data.
