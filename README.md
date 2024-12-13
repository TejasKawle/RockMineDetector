
# Rock vs Mine Detection System

This project implements a machine learning model to classify objects as either rocks or mines based on sonar data. It uses logistic regression to build and evaluate the model.

## Dataset

The dataset used in this project is the **Sonar Data Set**, which contains 60 frequency-based attributes representing sonar signals. Each data point is labeled as:
- **R**: Rock
- **M**: Mine

### Dataset Features
- 60 columns represent frequency responses.
- The 61st column is the label (`R` or `M`).

## Installation and Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   ```
2. Navigate to the project directory:
   ```bash
   cd <repo-name>
   ```
3. Install the required libraries:
   ```bash
   pip install pandas numpy scikit-learn
   ```
4. Open the Jupyter Notebook or run the script in your preferred environment (e.g., Google Colab).

## Project Workflow

### 1. Data Loading
The dataset is loaded into a Pandas DataFrame. The labels and features are separated for processing.

### 2. Data Splitting
The data is split into training and testing sets (90% training, 10% testing) while maintaining the class distribution using `train_test_split`.

### 3. Model Training
A Logistic Regression model is trained on the training data.

### 4. Model Evaluation
The model's accuracy is calculated on both the training and testing datasets.

### 5. Prediction System
A custom prediction system allows you to input new sonar data and classify it as a rock or a mine.

## Results

- **Training Accuracy**: ~83%
- **Testing Accuracy**: ~83%

## Example Prediction

Input data:
```python
input_data = (
    0.0130, 0.0120, 0.0436, 0.0624, 0.0428, 0.0349, 0.0384, 0.0446, 0.1318, 0.1375,
    0.2026, 0.2389, 0.2112, 0.1444, 0.0742, 0.1533, 0.3052, 0.4116, 0.5466, 0.5933,
    0.6663, 0.7333, 0.7136, 0.7014, 0.7758, 0.9137, 0.9964, 1.0000, 0.8881, 0.6585,
    0.2707, 0.1746, 0.2709, 0.4853, 0.7184, 0.8209, 0.7536, 0.6496, 0.4708, 0.3482,
    0.3508, 0.3181, 0.3524, 0.3659, 0.2846, 0.1714, 0.0694, 0.0303, 0.0292, 0.0116,
    0.0024, 0.0084, 0.0100, 0.0018, 0.0035, 0.0058, 0.0011, 0.0009, 0.0033, 0.0026
)
```
Output:
```
The object is a mine.
```

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn

## How to Use

1. Load the project in your environment.
2. Modify the input data in the `input_data` variable for new predictions.
3. Run the script or notebook to view predictions and model performance.

## Repository

Find the project repository [here](https://github.com/<your-username>/<repo-name>).

## License

This project is licensed under the MIT License.
