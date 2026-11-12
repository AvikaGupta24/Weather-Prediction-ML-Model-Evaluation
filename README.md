# Weather-Prediction-ML-Model-Evaluation
A machine learning capstone comparing KNN, Logistic Regression, Decision Tree and Random Forest classifiers on a synthetic weather dataset sourced from Kaggle, using accuracy, precision, recall and confusion matrices.

Four classification algorithms—K-Nearest Neighbors (KNN), Logistic Regression, Decision Tree and Random Forest—are trained and evaluated to determine their relative effectiveness in identifying weather categories.

The project examines each model's strengths, limitations and predictive performance using test accuracy, precision, recall and confusion matrices. Based on the comparative evaluation, Random Forest is identified as the best-performing model in this experiment.

## Objectives
- Explore and preprocess a weather classification dataset.
- Train and compare four supervised classification algorithms.
- Evaluate model performance using multiple classification metrics.

## Dataset
This project uses a synthetic weather classification dataset obtained from Kaggle. The dataset contains artificially generated weather observations rather than measurements collected from real-world meteorological stations.

The dataset includes features such as temperature, humidity, wind speed, precipitation, cloud cover, atmospheric pressure, UV index, season, visibility and location type.

The target label is Weather Type, with four possible classes: Sunny, Rainy, Cloudy and Snowy.

Source: [(https://www.kaggle.com/datasets/nikhil7280/weather-type-classification)]
Dataset creator: [Nikhil Narayan]

Limitation: Since the dataset is synthetic, model performance on its test split should not be interpreted as evidence of equivalent accuracy on real-world weather data.

## Methodology

1. Exploratory Data Analysis
The dataset was examined to understand its structure, feature types, missing values and potential relationships between variables.

2. Data Preprocessing
Categorical features were numerically encoded, and the dataset was divided into training and testing subsets using a stratified 75:25 split.
StandardScaler was fitted to the training features and applied to both training and testing data.

3. Model Development
Four classification algorithms were implemented:
K-Nearest Neighbors: Classifies observations based on the labels of nearby data points.
Logistic Regression: Provides a linear classification baseline.
Decision Tree: Learns hierarchical decision rules from the input features.
Random Forest: Combines multiple decision trees to produce ensemble predictions.

4. Model Evaluation
Models were compared using training and test accuracy, weighted precision, weighted recall and confusion matrices.
Additional experiments investigated KNN neighbour counts, Random Forest tree counts and feature importance.

## Results
Random Forest achieved the highest test accuracy, precision and recall among the four models evaluated.
KNN and Decision Tree demonstrated comparable performance, while Logistic Regression produced the lowest scores in this experiment.

## Conclusion
The project demonstrates the importance of algorithm comparison and multiple evaluation metrics when selecting a machine learning model.

However, further validation using real-world meteorological data would be necessary before making claims about practical weather prediction reliability.

## Technologies and Libraries Used:
Python
Pandas and NumPy
Scikit-learn
Matplotlib
Jupyter Notebook

## Running the Notebook
1. Clone or download this repository.
2. Install the required Python packages using pip install -r requirements.txt.
3. Open notebooks/Capstone_Weather.ipynb in Jupyter Notebook or a compatible environment.
4. Ensure the dataset is available at the path referenced in the notebook.
5. Run the notebook cells sequentially to reproduce the analysis and model comparisons.

### Project Type
Machine Learning Capstone Project — Supervised Classification and Comparative Model Evaluation.
