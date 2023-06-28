# <p align = 'center'>Cross-Sell Prediction</p>

## PROBLEM STATEMENT
The client is an insurance company that previously provided health insurance to customers. They are now seeking assistance in developing a predictive model to determine whether policyholders from the previous year would also be interested in purchasing vehicle insurance from the company.

In the context of insurance, a policy refers to an agreement in which an insurance company agrees to provide compensation for specific losses, damages, illnesses, or death in exchange for the payment of a predetermined premium. The premium is the amount of money that the customer must pay on a regular basis to the insurance company in order to receive this guarantee.

Similar to medical insurance, vehicle insurance requires customers to pay a yearly premium to an insurance provider company. This payment guarantees that in the event of an unfortunate accident involving the vehicle, the insurance provider company will offer compensation, also known as a "sum assured," to the customer.

Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

Now, in order to predict, whether the customer would be interested in Vehicle insurance, you have information about demographics (gender, age, region code type), Vehicles (Vehicle Age, Damage), Policy (Premium, sourcing channel) etc.

## Information about features in dataset
id : Unique ID for the customer

Gender : Gender of the customer

Age : Age of the customer

Driving_License 0 : Customer does not have DL, 1 : Customer already has DL

Region_Code : Unique code for the region of the customer

Previously_Insured : 1 : Customer already has Vehicle Insurance, 0 : Customer doesn't have Vehicle Insurance

Vehicle_Age : Age of the Vehicle

Vehicle_Damage :1 : Customer got his/her vehicle damaged in the past. 0 : Customer didn't get his/her vehicle damaged in the past.

Annual_Premium : The amount customer needs to pay as premium in the year

PolicySalesChannel : Anonymized Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.

Vintage : Number of Days, Customer has been associated with the company

Response : 1 : Customer is interested, 0 : Customer is not interested

## Metrics of Models used

![Screenshot 2023-06-28 151544](https://github.com/ImRupeshKsahu/Cross-sell-prediction/assets/137479496/91aaffbb-376d-466a-ae1f-705cfcbe7fce)

## Conclusions

The aim of this project was to predict whether customer would be interested in buying a Vehicle insurance or not.

Following insights came out:

87.7% customers responded as No for buying a vehicle insurance. It clearly shows that most of the customers are not interested in buying a vehicle insurance.

Males are 30% more likely to respond as yes for vehicle insurance than females. So company could focus more on targeting male customers and do more promotions targeted towards the female customers.

Most of the customers have driving license and out of them 12% are likely to respond as yes for vehicle insurance.

There is no point in reaching out to customers who already have vehicle insurance as almost all of them responded negatively for buying another insurance.

22% of customers responded positively who don't have previous insurance. So, company should focus more such customers as conversion possibility is higher is such cases.

Company should focus on customers whose vehicle is more than 2 years old, as 30% of times they are interested in buying an insurance, which is huge compared to other features.

Customers with vehicle age less than an year are least interested in insurance as while buying the vehicle people often buy 1 year insurance. Company shouldn't spend more time on these customers as just 4% of times they are likely to say Yes for a vehicle insurance.

Customers who damaged their vehicles in past are more sensitive towards buying a vehicle insurance. Infact 24% of times they responded positively based on this dataset.

Customers who haven't damaged their vehicle in past, almost all of the times they respond as No for insurance. In order to increase the customer base company could focus on conveying importance of a vehicle insurance to such customers.

Number of days customer associated with company has no impact on response by customers. Company should try building rapport, trust with old customers and could offer them extra perks while buying new products.

Based on our data, customers in the age group 31 to 60 have very high postive response rate compared to the younger and older customers. We also saw that customers in this age group are more likely to damage their vehicle and people with damaged vehicles are more likely to buy a vehicle insurance. So, this is a very good filter for company to target customers with high conversion rate.

Vehicle damage, previously insured, policy sales channel, age etc. are the most important features for predicting the response.

Driving license, gender, vintage etc. featues have no significant impact on predicting the response.

This dataset is the clear case of imbalance and we applied oversampling techniques such as SMOTE to help us improve the training data and hence the model prediction.

Logistic regression has highest recall for test data. So, if company needs a very high recall rate, i.e. lowest False Negatives then they may consider using logistic regression for prediction.

In test data we weren't able to maintain the high precision for 1 but recall, which is most important parameter in this cross sell prediction is above 85% for both Random Forest and XGboost along with 70% recall for 0s.

Random forest and XGboost after hyperparameter tuning have highest f1 score of 44% on test data and their test recall is also very high.
