# Iris_Data_Prediction

## 1. Data Preprocessing
### Exploratory Data Analysis (EDA)
Visualization Tools: We utilized Matplotlib and Seaborn for our visualizations.
Initial Data Inspection: We examined the dataset to understand the types of features, checked for missing values, and assessed the distribution of each feature. Plots such as histograms, box plots, and scatter plots were used to visualize the data.

### Outlier Detection and Handling
Interquartile Range (IQR) Method: Outliers were identified using the IQR method:
Lower Bound: Q1 - 1.5 * IQR
Upper Bound: Q3 + 1.5 * IQR
Values outside these bounds were considered outliers and were replaced with the respective lower or upper bound values. This approach helped in maintaining the integrity of the data while managing extreme values.

### Feature Scaling
Standard Scaler: Standard Scaler was applied to normalize the features. This transformation ensured that the features had a mean of 0 and a standard deviation of 1. Normalization is important for many machine learning algorithms, including Decision Tree Classifiers, as it ensures all features contribute equally to the decision process.

## 2. Model Training
### Decision Tree Classifier
Model Selection: A Decision Tree Classifier was chosen for its ability to handle non-linear relationships and its interpretability.
Training and Testing: The preprocessed data was split into training and testing sets. The Decision Tree Classifier was trained on the training set.
Evaluation: The model achieved an accuracy of 92% on the test set, demonstrating a strong predictive capability. This high level of accuracy indicates that the preprocessing steps, including outlier imputation and feature scaling, were effective in preparing the data for the Decision Tree Classifier.

## Conclusion
The meticulous preprocessing of the Iris dataset, encompassing outlier imputation using the IQR method and standard scaling of features, laid a solid foundation for the Decision Tree Classifier. This robust approach facilitated the model in achieving a notable accuracy of 92%, underscoring the significance of thorough data preparation in enhancing model performance.
