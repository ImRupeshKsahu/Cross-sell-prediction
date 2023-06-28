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

