# Airline-Satisfaction-Predictions
This project analyzes a massive airline survey to understand what drives customer loyalty. It looks at passenger details—like age, flight distance, and delays—to predict whether a passenger will be satisfied or dissatisfied. The goal is to help airlines figure out exactly which services (like Wi-Fi or legroom) need the most improvement.





## Objective

- Understand the data and preform the necessary cleaning
- Prepare te csv file for modeling
- Build a model to predict passenger Satisfaction



## Summary 

The airline should Reduce airplane for Eco and Eco Plus class and improve Eco and Eco Plys class customers Expereince such as adding more leg room for custumers and make it easy to buy a ticket online.



## Key Visualization 
### Visualization 1:
About half of the passengers ere unsatisified with the serivice they received with the biggest 3 problems being 
- Ease of Online Booking
- More Leg Room
- Better Baggage handling

![average flight](/images/average%20flight.jpg)

### Visualization 2:
The data suggest that most of passenger are unhappy in Eco Class but Business passengers are mostly satisfied.

![delay by satisfaction](/images/Delay_by_satisfaction.png)

### Base Model

For the base model, no scaler or transformer was used the same test size and random state for the final model settings stayed the same. 


| Mode                | Accurey Score |
| ------------------- | ------------- |
| Logistic Regreesion | 0.87          |
| Random Forest       | 0.96          |
| SV                  | 0.94          |


### Model
For the final model, the random state was set at 42 with a test_size of 0.2.Next, Standard Scaler was used to fit X and Y. Logistic regession was set at the `max iter`. The random forest, random state is the same and `n_estimator` at 200. 


| Mode                | Score |
| ------------------- | ----- |
| Logistic Regreesion |  0.87     |
| Random Forest       |  0.96     |
| SV                  |  0.95     |


![model preformance](/images/model_preform_1.png)



