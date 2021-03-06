# MAIS202_FinalProject
Includes all project deliverables for MAIS202 Winter 2020 and the final webapp.

First, the design process folder contains all the deliverables that I submitted throughout MAIS202. It serves as documentation on my design process.

The Used_Car_Predictor release contains all the code and trained data to run or repreduce my webapp.  

Here is a short description of the project:
Evaluating and comparing prices of used cars can be challenging and very time consuming for customers. I built a project that predicts the price of used cars from 38 different brands based on their make, model, year and mileage. The goal of the project is to estimate the price that a customer should expect to pay for a car based on past selling data. This application should not be used by resellers or car dealership since the predicted price are not precise enough to justify buying a car or not. For instance, since my moel does not take into account any options on the cars, it will always predict the same price for a given model (assuming constant year and mileage). This is not true in reality as some options can greatly affect the value of used cars.

The data for the project was obtained from Kaggle. Someone trying to replicate my project should downoad the dataset from the following address: https://www.kaggle.com/jpayne/852k-used-car-listings. I used a random forest regressor from Scikit-Learn to build my model. The model was trained with the data of 1.2million used car sells in the US. Therefore, the predicted price is in USD and reflects the US market. I used the default hyperparameters for my model as they seemed to give me the best results from my preliminary tests and final test results (deliverable 2 and 3). Also, I built a random forest regressor for every make as that gave the best predictions based on my tests. The method I used to calculate the accuracy of my model was the percentage difference betwenn the predicted price and the real price of a car. 

Finally, I integrated my training weights in an interactive web application. My final product has an average error of 8% between the real price and the predicted price of a car. This error can be further broken down on a per make basis. To run the final project, one should follow the instructions given in the Used_Car_Predictor release.
