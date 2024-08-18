# Coronary Heart Disease Prediction Project

## Theoretical Background

The objective of this project is to predict the 10-year risk of coronary heart disease (CHD) using data from the Framingham Heart Study. Coronary heart disease is a leading cause of death worldwide. Predicting CHD risk can help in early intervention and management, ultimately reducing the burden of the disease.

### Coronary Heart Disease (CHD)
Coronary heart disease occurs when the coronary arteries become narrowed or blocked due to plaque buildup (atherosclerosis). This can lead to chest pain, heart attacks, and other cardiovascular events. Risk factors include high blood pressure, high cholesterol, smoking, diabetes, obesity, physical inactivity, and family history of heart disease.

### The Framingham Heart Study
The Framingham Heart Study is a long-term study focused on cardiovascular disease. The dataset used in this project is a subset containing 4240 observations and 16 variables, including demographic information, risk factors, and the 10-year risk of CHD.

### Predictive Modeling
The project uses neural networks as the main predictive modeling technique, with a focus on addressing imbalanced data, which is common in healthcare datasets. Techniques like SMOTE, undersampling, and class weighting were applied to handle the imbalance.

### Imbalanced Data Techniques
- **SMOTE:** Oversampling the minority class.
- **Undersampling:** Reducing instances of the majority class.
- **Class Weights:** Adjusting weights during model training.

### Model Evaluation Metrics
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**

## Methodological Description

### Exploratory Data Analysis (EDA)
EDA was conducted to understand the data distribution and relationships between variables. Sweetviz was used for generating comprehensive visualizations.

### Data Preprocessing
Steps included handling missing values, transforming skewed variables, and normalizing the data.

### Data Splitting
The dataset was split into training, validation, and test sets. The data was standardized using `StandardScaler`.

### Model Training and Evaluation
Multiple models were trained, including neural networks, random forest, and gradient boosting. Techniques like SMOTE and undersampling were applied to handle class imbalance.

### Visualization
Bar charts and confusion matrices were used to evaluate model performance.

### Libraries and Tools Used
- **Pandas**: Data manipulation
- **NumPy**: Numerical computations
- **Matplotlib & Seaborn**: Visualization
- **TensorFlow & Keras**: Neural networks
- **Scikit-learn**: Machine learning algorithms
- **Imbalanced-learn**: Handling imbalanced datasets
- **Sweetviz**: Automated EDA

## Results and Evaluation

The models were evaluated using precision, recall, F1-score, and accuracy. The best-performing model was Model 7, which used neural networks combined with undersampling, demonstrating strong performance in predicting the minority class (CHD).

### Final Model Selection
Model 7 was chosen due to its balanced performance across metrics and its consistency on both validation and test data.

### Conclusion
While Model 7 performed well, there is room for improvement, particularly in precision and recall. Future work includes expanding the dataset and exploring advanced techniques for handling imbalanced data.

## Resources
- [Kaggle Dataset](https://www.kaggle.com/datasets/dileep070/heart-disease-prediction-using-logistic-regression)

