# House Price Prediction Project

## 📖 Project Overview
This project focuses on building machine learning models to predict house prices based on various property features. The project follows a structured data science workflow from data exploration and preprocessing to model training and evaluation.

**Dataset Source:** [House Prediction Dataset from Kaggle](https://www.kaggle.com/datasets/zafarali27/house-price-prediction-dataset)

## 📊 Dataset Description
The dataset contains 2,000 property records with the following features:

| Feature | Description | Type |
|---------|-------------|------|
| Id | Unique identifier for each property | Numerical |
| Area | Area of the property (sq. ft.) | Numerical |
| Bedrooms | Number of bedrooms | Numerical |
| Bathrooms | Number of bathrooms | Numerical |
| Floors | Number of floors | Numerical |
| YearBuilt | Year the property was built | Numerical |
| Location | Area where property is located | Categorical |
| Condition | Condition of the property | Categorical |
| Garage | Whether property has a garage | Categorical |
| Price | Target variable: Sale price | Numerical |


## 📈 Key Findings

### Data Quality
- The dataset contains no missing values
- No significant outliers were detected in numerical features
- All data types are appropriate for the features

### Model Performance
Three models were evaluated:

| Model | MSE (×10⁹) | R² Score | Observation |
|-------|------------|----------|-------------|
| Linear Regression | 78.66 | -0.011 | Best performer but still poor |
| Decision Tree | 167.22 | -1.149 | Severe overfitting |
| Random Forest | 82.68 | -0.063 | Better than single tree but still poor |

**Note:** Negative R² values indicate all models perform worse than simply predicting the mean house price.

## 🎯 Results Interpretation
The initial modeling approach did not yield satisfactory results. The models failed to capture the complex relationships in the data. Key insights:
- Linear relationships are insufficient for this prediction task
- Decision Trees overfit severely without proper regularization
- Feature engineering and more sophisticated models are needed

## 🔮 Next Steps & Recommendations
1. **Feature Engineering**: Create new features like property age, room ratios, etc.
2. **Advanced Models**: Experiment with Gradient Boosting (XGBoost, LightGBM) and Neural Networks
3. **Hyperparameter Tuning**: Implement systematic tuning for model optimization
4. **Additional Data**: Collect more relevant features that influence house prices


## 📝 License
This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments
- Dataset provided by Kaggle user zafarali27
- Built with Python's data science ecosystem (pandas, scikit-learn, matplotlib)
