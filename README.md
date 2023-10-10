# 🏡 HousingPrices: Predict if a House is Expensive or Not

Welcome to the HousingPrices repository! In this project, we harness the power of 80 unique features to predict whether a house is expensive or not. A binary classification problem at its core, this project offers insights into data preprocessing, model selection, and hyperparameter tuning.

## 🗂️ Data Files

- housing-classification: This dataset serves as the foundation for building and training our model.
- test: An unseen dataset used to evaluate our model. Predictions from this dataset were uploaded to the platform for evaluation.
- data description: Dive deep into this file to understand the nuances and descriptions of each feature in the datasets.

All data files can be found in the data folder.

## 📓 Notebooks in this Repository

1. Model Selection Notebook: Dive deep into the exploration and comparison of different machine learning models to find the best one for our data.
2. Model Application & Tuning Notebook: Embark on the journey of applying the chosen model, tuning its parameters, and enhancing its performance.

After rigorous testing, the XGBoost model emerged as the top performer and was selected for further tuning and application.

## 🚀 Model Pipeline

Here's a brief rundown of the steps in our final model pipeline:

1. Numerical Data Processing:
- 🔄 SimpleImputer: Fills in missing values.

2. Categorical Data Processing:
- 🔄 SimpleImputer: Deals with missing categorical data.
- 🌐 OneHotEncoding & OrdinalEncoding: Transform categorical data into a format suitable for machine learning.

3. Scaler: Use a scaler if opting for the ASDYN oversampler.

4. Oversampling: The ASDYN oversampler is our choice, as it showcased a significant improvement in model performance. You can validate this claim with the loop included in the notebook.

5. Feature Selection: To cherry-pick the most relevant features for the model and avoid the treacherous path of overfitting.

6. Model Application: Finally, deploy the XGBClassifier to predict our desired outcome.

> **Note**: Throughout the project, we've adhered to a random_state of 42 to ensure reproducibility.

## ⚙️ Hyperparameter Tuning

To extract the maximum potential from our model:

1. We initialized our search using the RandomSearchCV, navigating through a vast parameter space efficiently.
2. Fine-tuning was then performed using GridSearchCV with a refined parameter grid, ensuring our model is tuned to its optimum.

## 📊 Final Results

Upon predicting unseen data (for which actual results were unknown), our model secured an impressive accuracy of 0.9756. While we're thrilled with the outcome, we're always on the lookout for ways to elevate our performance in future endeavors.

## 🔄 Usage

1. Clone this repository.
2. Navigate to the data folder and familiarize yourself with the datasets.
3. Proceed to the notebooks and run them in sequence.
4. Adjust hyperparameters or model settings as needed.

## 🎉 Conclusion

Thank you for visiting this repository. We hope it provides valuable insights and paves the way for your future data science projects. Happy coding and here's to making better predictions! 🚀
