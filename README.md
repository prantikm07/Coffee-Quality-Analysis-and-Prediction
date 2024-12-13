# Coffee Quality Prediction using Machine Learning

This project aims to predict the quality of coffee based on various sensory attributes such as sweetness, acidity, aroma, flavor, body, and balance. The model utilizes machine learning algorithms and Principal Component Analysis (PCA) for feature reduction to build accurate prediction models.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Data Preprocessing](#data-preprocessing)
- [Feature Engineering](#feature-engineering)
- [Machine Learning Models](#machine-learning-models)
- [Evaluation Metrics](#evaluation-metrics)
- [Results and Visualization](#results-and-visualization)
- [Installation Instructions](#installation-instructions)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The project uses machine learning techniques to predict the "Total Cup Points" of coffee. These points are based on different sensory parameters like sweetness, aroma, flavor, acidity, balance, and more, which are evaluated by coffee tasters. Using regression models, we aim to predict this continuous value.
The approach also integrates Principal Component Analysis (PCA) for dimensionality reduction to explore how reducing the feature space affects the performance of machine learning models.

## Dataset

The dataset contains the following features:
- **Sweetness**: The sweetness level of the coffee (0-10 scale).
- **Acidity**: The level of acidity in the coffee (0-10 scale).
- **Aroma**: The aroma strength of the coffee (0-10 scale).
- **Flavor**: The flavor rating of the coffee (0-10 scale).
- **Body**: The body or mouthfeel of the coffee (0-10 scale).
- **Balance**: The balance between the flavors (0-10 scale).
- **Aftertaste**: The aftertaste rating of the coffee (0-10 scale).
- **Uniformity**: The uniformity in the taste of the coffee (0-10 scale).
- **Clean Cup**: The clarity of the coffee (0-10 scale).
- **Total Cup Points**: The overall evaluation score of the coffee (0-100 scale).

## Technologies Used

- **Python**: Programming language for data analysis and machine learning.
- **Pandas**: For data manipulation and analysis.
- **Scikit-learn**: For machine learning algorithms and preprocessing.
- **XGBoost**: For advanced gradient boosting models.
- **Matplotlib** and **Seaborn**: For data visualization.
- **NumPy**: For numerical operations.
- **PCA**: For dimensionality reduction of features.
  
## Data Preprocessing

1. **Handling Missing Data**: The dataset is first cleaned by removing or imputing missing values.
2. **Scaling**: The numeric data is scaled using `StandardScaler` to standardize features before training models.
3. **PCA**: Principal Component Analysis (PCA) is applied to reduce dimensionality, improving model performance and interpretability.

## Feature Engineering

We focus on transforming the raw features into meaningful patterns that help the models predict the "Total Cup Points" accurately. This includes scaling the data and applying PCA for dimensionality reduction.

## Machine Learning Models

We use the following machine learning models for prediction:
- **Random Forest Regressor**: An ensemble learning method to predict continuous values.
- **XGBoost Regressor**: A more advanced model based on gradient boosting.
- **Linear Regression**: A basic regression model used for comparison.

## Evaluation Metrics

To evaluate the performance of the models, the following metrics are used:
- **Mean Absolute Error (MAE)**: The average of the absolute errors between predicted and actual values.
- **Mean Squared Error (MSE)**: The average of the squared errors between predicted and actual values.
- **R² Score**: Measures the proportion of variance in the dependent variable explained by the model.
- **Mean Absolute Percentage Error (MAPE)**: A measure of prediction accuracy in percentage terms.

## Results and Visualization

The results of the models are visualized using:
- **Scatter plots**: To compare actual vs predicted values for different models.
- **Heatmaps**: To visualize the correlation matrix between features and the target variable.
- **Cumulative Variance Plot**: To visualize how much variance in the data can be explained by each principal component after PCA.

## Installation Instructions

Follow these steps to install the necessary dependencies for running the project:

1. Clone the repository:
   ```bash
   https://github.com/prantikm07/Coffee-Quality-Analysis-and-Prediction.git
   cd coffee-quality-prediction
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   ```

3. Activate the virtual environment:
   - **Windows**: `.\venv\Scripts\activate`
   - **Mac/Linux**: `source venv/bin/activate`



## Usage

Once the dependencies are installed, you can run the script for data preprocessing, training models, and making predictions.

To execute the main script:
```bash
python main.py
```

This will run the analysis, train the models, and display the evaluation results.

## Contributing

We welcome contributions to this project. To contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Author - [Prantik Mukhopadhyay](https://www.linkedin.com/prantikm07)
