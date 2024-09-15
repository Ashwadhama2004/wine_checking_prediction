# wine_checking_prediction





This project involves predicting the quality of red wine using a machine learning approach. The dataset contains various chemical properties of the wine, and the target is the wine quality, which is rated on a scale from 0 to 10. The quality ratings are classified into two categories: good (quality >= 7) and bad (quality < 7). The project employs two models: Random Forest Classifier and Support Vector Machine (SVM) for prediction.

## Dataset

The dataset used is `winequality-red.csv`, which consists of the following columns:
- **fixed acidity**
- **volatile acidity**
- **citric acid**
- **residual sugar**
- **chlorides**
- **free sulfur dioxide**
- **total sulfur dioxide**
- **density**
- **pH**
- **sulphates**
- **alcohol**
- **quality** (target variable)

The dataset has no missing values, and the target variable `quality` is split into two classes:
- `1` for good quality (quality >= 7)
- `0` for bad quality (quality < 7)

## Models

Two models are trained to predict wine quality:
1. **Random Forest Classifier**
2. **Support Vector Machine (SVM)**

### Random Forest Classifier
- Achieved **100% accuracy** on the training set.
- Achieved **90.63% accuracy** on the test set.

### SVM (Support Vector Classifier)
- Achieved **86.40% accuracy** on the training set.
- Achieved **86.56% accuracy** on the test set.

## Dependencies

The project uses the following Python libraries:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

## Installation

1. Clone the repository:
   ```bash
   git clone <https://github.com/Ashwadhama2004/wine_checking_prediction/tree/main>
   cd <repository-directory>
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure that the dataset `winequality-red.csv` is in the project directory.

## Usage

To run the wine quality prediction:
1. Load the dataset and explore the data.
2. Train the models using the training dataset.
3. Predict the wine quality for the test data or any custom input.

```python
input_data = (7.3, 0.65, 0.0, 1.2, 0.065, 15.0, 21.0, 0.9946, 3.39, 0.47, 10.0)
```

Use the trained Random Forest or SVM model to predict the wine quality:

- For Random Forest Classifier:
   ```python
   prediction = model.predict(input_data)
   ```

- For SVM:
   ```python
   prediction = model_svm.predict(input_data)
   ```

The model will output whether the wine is of **good quality** or **bad quality** based on the input features.

## Results

- The **Random Forest Classifier** performed better, achieving higher accuracy on both training and test sets compared to the SVM model.
- The project also includes visualizations such as bar plots and a heatmap to show the relationships between different features and the target variable.

## Conclusion

This project demonstrates the application of machine learning models to classify wine quality based on its chemical properties. The Random Forest model outperformed SVM in predicting wine quality.

---
License
This project is licensed under the MIT License - see the LICENSE file for details.
