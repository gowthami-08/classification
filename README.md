# classification
1. Importing Libraries
Essential libraries for data manipulation (pandas, numpy), visualization (seaborn, matplotlib), and machine learning (scikit-learn) are imported.

2. Loading the Dataset
The Breast Cancer Wisconsin dataset is loaded from the CSV file.

3. Initial Data Inspection
.head() is used to preview the data.

isnull().sum() is used to check for missing values.

A heatmap is plotted to visualize missing values.

4. Data Cleaning
Unnecessary columns like 'id' and 'Unnamed: 32' are dropped.

5. Encoding Target Variable
The 'diagnosis' column is encoded:

'M' (Malignant) → 1

'B' (Benign) → 0

Converted to categorical type for clarity.

6. Visualizing Target Variable
A bar plot shows the distribution of malignant vs benign cases.

7. Splitting Features and Target
X = features (all columns except diagnosis)

y = target (diagnosis column)

8. Feature Scaling
Used StandardScaler to normalize the features (important for models like Logistic Regression).

9. Train-Test Split
Split the dataset: 70% training, 30% testing (using train_test_split).

Metric	Meaning
Confusion Matrix	Shows TP, FP, TN, FN
Accuracy	(TP + TN) / Total samples
Precision	TP / (TP + FP)
Recall (Sensitivity)	TP / (TP + FN)
F1 Score	Harmonic mean of precision and recall
ROC AUC Score	Area under the ROC curve; closer to 1 is better
ROC Curve	Trade-off between sensitivity and specificity

