🏠 House Price Prediction
📌 Overview

This project applies machine learning to predict house prices.
It uses Linear Regression as the model and demonstrates a workflow including data preprocessing, feature engineering, training, evaluation, and generating predictions for submission.

📂 Dataset

The project works with three datasets:

train.csv → Training data with both features and target variable (SalePrice).

test.csv → Test data with only features (to be predicted).

sample_submission.csv → Template showing the required format for predictions.

⚙️ Data Preprocessing & Feature Engineering

To improve model performance:

Missing values are handled properly.

A new feature called TotalBaths is engineered by combining multiple bathroom-related columns (FullBath, HalfBath, BsmtFullBath, BsmtHalfBath).

Final features used for training:

GrLivArea → Above-ground living area (square feet).

BedroomAbvGr → Number of bedrooms above ground.

TotalBaths → Engineered total bathrooms.

🧠 Model Training

The dataset is split into training and validation sets.

A Linear Regression model is trained on the selected features.

The trained model is used to predict house prices on validation and test datasets.

📊 Model Evaluation

The model is evaluated using:

MAE (Mean Absolute Error) – Average error between predicted and actual values.

RMSE (Root Mean Squared Error) – Standard deviation of prediction errors.

R² Score – How much variance in the target variable is explained by the model.

🚀 Predictions

Predictions are generated for the test dataset.

Final results are saved into submission.csv in the required format.

🛠️ Tech Stack

This project is built with:

Python

NumPy – numerical operations

Pandas – data processing

Matplotlib – visualization

Scikit-learn – machine learning

📌 How to Run

Clone this repository.

Add the dataset files (train.csv, test.csv, sample_submission.csv) into the project folder.

Open and run the Jupyter Notebook (Task1.ipynb).

Evaluate the model performance.

Generate predictions → results will be stored in submission.csv.
