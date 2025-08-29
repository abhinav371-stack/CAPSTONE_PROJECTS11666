1. Project Overview:
SmartTech Co. partnered with our team to build a machine learning model that predicts laptop prices based on their specifications. The aim is to:
Enable accurate pricing
Understand key price drivers
Leverage brand perception in product strategy

2. Dataset Summary:
Total Records: 1273.
Features: Brand, RAM, CPU, GPU, Screen Resolution, Storage, etc.
Target: Price (in INR).

3. Data Cleaning & Preprocessing:
Dropped null and invalid entries (e.g., unknown weights).
Converted units ("8GB" → 8, "1.8kg" → 1.8).
Parsed and separated complex fields.
 Memory → SSD, HDD, Flash, Hybrid (in GB).
 CPU & GPU → extracted brand and series.
 Screen Resolution → width, height, touchscreen, PPI.
Categorical columns one-hot encoded.

4. Feature Engineering:
Newly Added Features:
  Touch Screen, IPS, Resolution Width, PPI, Height.
  CPU _ Brand, CPU _ Series, GPU _ Brand.
  SSD, HDD, Flash Storage, Hybrid.

5. Model Development:
Trained the following regression models:
  Linear Regression Model
  Random Forest Regressor Model
  KNN Regressor 
  SVR Regressor
  Decision Tree Regressor
Performance Comparison:
                                 MAE                 RMSE          R^2 SCORE
   LINEAR REGRESSION           11576.87            17017.13         0.7396
   RANDOM FOREST REGRESSOR     8033.81             13271.23         0.8416
   KNN                         11982.27            18958.57         0.6767
   SUPPORT VECTOR              9738.29             17494.83         0.7247
   DECISION TREE               25629.71            33340.97         0.0003

From the above data we can say that the best model for this prediction is
RANDOM FOREST REGRESSOR

6. Hyperparameter Tuning:
Used GridSearchCV to tune the Random Forest model and improved R2 to 84.18%.

7. Conclusion:
After studying the ML model we came to some conclusions that are mentioned in the next slide. We came across some limitations while deciding the prices and we successfully overcome them by implementing good techniques.

The developed model helps SmartTech Co.:

Predict prices accurately.
Understand the components impacting value.
Strategically design and price future products.
















