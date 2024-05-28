# Introduction to Machine Learning: Assignment #1

This project implements various machine learning algorithms, including Naïve Bayes, Gaussian Bayes, Parzen Windows, and K-Nearest Neighbors (KNN). The code performs data preprocessing, training, evaluation, and visualization for multiple datasets.

## Requirements

- Python 3.x
- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn
- tqdm

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/ml-assignment1.git
    cd ml-assignment1
    ```

2. Install the required libraries:
    ```sh
    pip install numpy pandas matplotlib seaborn scikit-learn tqdm
    ```

## Usage

### Naive Bayes

1. **Data Preparation:**
    ```python
    url = 'path/to/emotions_train.csv'
    df = pd.read_csv(url)
    ```

2. **Training and Classification:**
    ```python
    Pw, P = learn_NB_text()
    sum_right = ClassifyNB_text(Pw, P)
    print(sum_right)
    ```

### Gaussian Bayes

1. **Data Loading:**
    ```python
    url = "https://sharon.srworkspace.com/ml/datasets/hw1/banknote_authentication.csv"
    df = pd.read_csv(url)
    ```

2. **Training and Evaluation:**
    ```python
    accs = classify_point_gaussian_bayes(x_train)
    ```

3. **Visualization:**
    ```python
    plt.contourf(xx, yy, Z, alpha=0.8)
    plt.scatter(X_reduced[:, 0], X_reduced[:, 1], c=y_train, cmap=plt.cm.RdYlBu)
    plt.show()
    ```

### K-Nearest Neighbors

1. **Data Loading and Preprocessing:**
    ```python
    url = "https://sharon.srworkspace.com/ml/datasets/hw1/Stars.csv"
    star_data = pd.read_csv(url, sep=";")
    df = star_data.dropna()
    ```

2. **Training and Evaluation:**
    ```python
    predictions = kNN_classify(X_train, y_train, X_test, k)
    ```

3. **Visualization:**
    ```python
    plt.figure(figsize=(12, 6))
    plt.plot(ks, accs, label='Accuracy', color='blue')
    plt.show()
    ```

## License

This project is licensed under the MIT License.
