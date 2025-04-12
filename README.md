# Cars_Purchasing
🚗 Car Purchase Prediction Using Machine Learning and ANN 📌 Objective  The objective of this project is to predict the amount a customer is likely to spend on purchasing a car based on their demographic and financial data, using both traditional machine learning (Linear Regression) and a deep learning approach (Artificial Neural Network).
📁 Dataset Overview

    Source: car_purchasing_data.csv

    Features:

        Gender

        Age

        Annual Salary

        Credit Card Debt

        Net Worth

    Target Variable:

        Car Purchase Amount

The dataset also includes non-informative fields such as Customer Name, Customer e-mail, and Country, which were dropped during preprocessing.
🔍 Exploratory Data Analysis (EDA)

    Used boxplot and pairplot to visualize relationships and detect outliers.

    Scatter plot between Annual Salary and Car Purchase Amount showed a visible positive correlation.

    Verified that the dataset had no missing values or duplicates.

⚙️ Data Preprocessing

    Feature Selection: Removed irrelevant columns.

    Scaling: Used MinMaxScaler to normalize both features (X) and target (y).

    Train-Test Split:

        80% training data

        20% testing data

        random_state=25 for reproducibility

📈 Model 1: Linear Regression

    Implemented using sklearn.linear_model.LinearRegression.

    Evaluated using R² Score and Root Mean Squared Error (RMSE).

    Coefficients and intercept analyzed to understand feature influence.

    Predictions made for test data and sample inputs.

🧠 Model 2: Artificial Neural Network (ANN)

    Built using Keras (TensorFlow backend).

    Architecture:

        Input Layer: 5 neurons (one per feature)

        Hidden Layers:

            Layer 1: 25 neurons (ReLU)

            Layer 2: 125 neurons (ReLU)

        Output Layer: 1 neuron (Linear activation)

    Loss Function: Mean Squared Error

    Optimizer: Adam

    Epochs: 22

    Batch Size: 25

    Included training-validation split (80/20) for performance tracking.

📊 Model Evaluation

    Visualized training and validation loss over epochs for the ANN.

    Compared performance:

        Linear Regression: Quick, interpretable, but less accurate.

        ANN: More complex, better fitting to data patterns, lower error rate.

Metrics:

    Linear Regression RMSE: ~calculated value

    ANN RMSE: ~calculated value

    R² Score: Compared for both models.

✅ Conclusion

    ANN outperformed Linear Regression in capturing the nonlinear relationships between customer financial features and car purchase amount.

    Project demonstrates the value of both traditional and deep learning models for regression tasks in business prediction scenarios.
