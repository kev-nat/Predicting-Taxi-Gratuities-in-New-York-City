# Predicting Taxi Gratuities in New York City

### **Overview**
<p align="justify"> The objective of this project was to develop multiple linear regression and random forest models to predict whether a rider would leave a high gratuity. The project analyzed yellow taxi trips in New York City from 2017. The final random forest model achieved an accuracy of 70% and a precision of 69%, identifying key features that distinguish low tippers from high tippers. The model revealed that the duration, distance, and cost of the trip were the most significant factors in determining whether a tip would exceed 20%. Automatidata is consulting for the New York City Taxi and Limousine Commission (TLC), which oversees the licensing and regulation of taxis and for-hire vehicles in the city. The TLC has partnered with Automatidata to create a regression model to estimate taxi fares before the ride, utilizing the data collected by the TLC. </p>

### **Business Understanding**
<p align="justify"> According to salary.com, New York taxi drivers earn an average salary of approximately $45,000. This income is notably low when compared to the median monthly rent of $6,500. To help drivers achieve a livable wage, it is crucial to understand the factors that motivate riders to leave tips. </p>

### **Data Understanding**
<p align="justify"> The data from the NYC Taxi and Limousine Commission, sourced from <a href="https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page">NYC.gov</a>, includes approximately 408,000 unique trips and 18 features. These features cover details such as trip duration, destination, vendor, toll information, and payment type. The bar chart below illustrates the distribution of generous tippers (those tipping over 20%) compared to non-generous tippers within the dataset. </p>

![image](https://github.com/user-attachments/assets/a70399a7-7d3d-477b-a79c-caadac580f9a)

<p align="justify"> In connection with this, a feature was engineered to represent whether a ride was taken during rush hour or not. Multiple redundant columns were dropped and reformatted into the proper data type. </p>

### **Modeling and Evaluation**
<p align="justify"> A random forest model comprising 400 decision trees was used to determine the feature importance in predicting who would tip generously or not. The plot below shows that VendorID, predicted_fare, mean_duration, and mean_distance were the top four most important factors in distinguishing a generous tipper from a non-generous one. The overall model performed with 70% accuracy and 69% precision. </p>

![image](https://github.com/user-attachments/assets/343159ee-aaa2-41de-ac13-1204de0689ca)

### **Conclusion**
<p align="justify"> 
This model can help taxi drivers by predicting the likelihood of receiving a generous tip. However, implementing a parametric model to assess the specific impact of each variable on the tip amount could provide more detailed insights. Additionally, incorporating data on a rider’s previous tipping behavior in future models could further assist stakeholders in resolving their business issues. </p>
