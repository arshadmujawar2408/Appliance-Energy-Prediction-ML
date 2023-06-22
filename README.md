# ML for Appliance Energy Prediction  
 The data set is at 10 min for about 4.5 months. The house temperature and humidity conditions were monitored with a ZigBee wireless sensor network. Each wireless node transmitted the temperature and humidity conditions around 3.3 min. Then, the wireless data was averaged for 10 minutes. The energy data was logged every 10 minutes with m-bus energy metres. Weather from the nearest airport weather station (Chievres Airport, Belgium) was downloaded from a public data set from Reliable Prognosis (rp5.ru) and merged together with the experimental data sets using the date and time column. Two random variables have been included in the data set for testing the regression models and to filter out non-predictive attributes You need to predict the energy use of appliances.

**Programming Language** : Python

**Libraries used** : Pandas, Numpy, Matplotlib, Seaborn, Sklearn, 

**NoteBook** : Google Colab

**Dataset Source** : Provided by Almabetter themself.
 
## Dataset 
We are given an Appliance Energy dataset. It contains the following features.
``` 
- Appliances :Dependant variable, energy use in Wh (watt-hour)
- lights :energy use of light fixtures in the house in Wh (watt-hour)
- T1 :Temperature in kitchen area, in Celsius
- RH_1 :Humidity in kitchen area, in %
- T2 :Temperature in living room area, in Celsius
- RH_2 :Humidity in living room area, in %
- T3 :Temperature in laundry room area, in Celsius
- RH_3 :Humidity in laundry room area, in %
- T4 :Temperature in office room, in Celsius
- RH_4 :Humidity in office room, in %
- T5 :Temperature in bathroom, in Celsius
- RH_5 :Humidity in bathroom, in %
- T6 :Temperature outside the building(north side), in Celsius
- RH_6 :Humidity outside the building(north side), in %
- T7 :Temperature in lroning room, in Celsius
- RH_7 :Humidity in lroning room, in %
- T8 :Temperature in teenager room 2, in Celsius
- RH_8 :Humidity in teenager room 2, in %
- T9 :Temperature in parent room, in Celsius
- RH_9 :Humidity in parent room, in %
- T_out :Temperature outside(from chievres weather station), in Celsius
- Press_mm_hg :pressure (from chievres weather station), in mm Hg
- RH_out :Humidity outside (from chievres weather station), in %
- windspeed :(from chievres weather station), in m/s
- visibility :(from chievres weather station), in km
- Tdewpoint : (from chievres weather station), in AC
- rv1 :Random variable 1, nondimensional
- rv2 :Random variable 2, nondimensional
```

- Total number of rows in data:  19735
- Total number of columns:  29 
  
## Exploratory Data Analysis
 Mainly performed using Matplotlib and Seaborn library and the following graph and plots had been used:
   - KDE Plot.
   - Scatter Plot.
   - Line Plot.
   - Heatmap.
   - Box Plot
   - Histogram
             
## ML Model Used:

Several machine learning algorithms were utilized in this project to predict the energy consumption of household appliances. These models include:
```
1. Support Vector Machine (SVM)
2. Random Forest
3. XGBoosLogistic Regression 
 ```
## Conclusion  
As a single person, I followed a standard workflow for data analysis and model building. Here's a summary of the steps I took:

- Dataset Understanding and EDA: I began by gaining a basic understanding of the dataset, exploring its contents, and performing Exploratory Data Analysis (EDA). This step helped me uncover valuable insights and characteristics of the dataset.

- Preprocessing: Based on the specific problems I wanted to address, I performed preprocessing on the dataset. This step involved handling missing values, handling outliers, scaling features, encoding categorical variables, and any other necessary data transformations.

- Feature Engineering: To enhance the predictive power of the models, I applied feature engineering techniques. This involved creating new features, selecting relevant features, or transforming existing features to improve their representation.

- Model Building: The core of my work was focused on building predictive models. I constructed three different models: Support Vector Machine (SVM), Random Forest, and XGBoost. Initially, I used the default parameters for each model.

- Hyperparameter Optimization: To improve the performance of the models, I employed various techniques to find optimal hyperparameters for each model individually. This could include techniques like grid search, random search, or Bayesian optimization.

- Model Evaluation: I used Root Mean Squared Error (RMSE) as the evaluation metric to compare the performance of the different models. The model with the lowest RMSE was considered the best among the three.

- Model Selection: Based on the evaluation results, I selected XGBoost as the preferred model due to its good performance on the dataset.

- Feature Importance: To gain insights into the contribution of each feature in the prediction task, I calculated feature importance using techniques specific to XGBoost or other applicable methods.

By following these steps, I was able to perform data analysis, build models and select the best model. 
