# Iris Flower Classification

This project implements a logistic regression model to classify iris flowers into three species (Setosa, Versicolor, Virginica) using the Iris dataset. The model is built using Python and Scikit-learn, with preprocessing steps including label encoding and feature scaling.

## Dataset
The [Iris dataset](https://archive.ics.uci.edu/ml/datasets/iris) contains 150 samples with 4 features (sepal length, sepal width, petal length, petal width) and a target variable (species). The dataset is stored in `iris.csv`.

## Prerequisites
- Python 3.6+
- Libraries: `pandas`, `numpy`, `scikit-learn`

Install dependencies using:
```bash
pip install pandas numpy scikit-learn
```

## Project Structure
- `iris.csv`: Input dataset
- `iris_classification.ipynb`: Jupyter notebook with the code
- `README.md`: This file

## Code Overview
1. **Load Data**: Reads `iris.csv` into a pandas DataFrame and sets `Id` as the index.
2. **Preprocessing**:
   - Features (`X`): Sepal length, sepal width, petal length, petal width
   - Target (`y`): Species (encoded as 0, 1, 2 using LabelEncoder)
   - Train-test split: 90% training, 10% testing
   - Feature scaling: StandardScaler applied to features
3. **Model Training**: Logistic regression model trained on scaled training data
4. **Evaluation**: Accuracy calculated on test predictions

## How to Run
1. Clone the repository:
   ```bash
   git clone <https://github.com/DakaBhai/Iris_Flower_Classification/tree/main>
   ```
2. Navigate to the project directory:
   ```bash
   cd <Iris_Flower_Classification>
   ```
3. Ensure `iris.csv` is in the project directory.
4. Open the Jupyter notebook:
   ```bash
   jupyter notebook iris_classification.ipynb
   ```
5. Run all cells to train the model and view the accuracy.

## Results
The model achieves high accuracy (typically >90%) on the test set, depending on the train-test split.

## Contributing
Feel free to fork this repository, make improvements, and submit pull requests. Suggestions for optimizing the model or adding new features are welcome!

## License
This project is licensed under the MIT License.
