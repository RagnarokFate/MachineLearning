# Introduction to Machine Learning: Assignment #4

## Submission Date: 31/07/2024, 23:55

### Topics:
- Ensemble methods
- AdaBoost
- PCA
- LDA
- K-means clustering


## Assignment Instructions:
- Submissions in pairs only.
- Try to keep the code as clean, concise, and short as possible.
- If you wish to work in your IDE, you can, but you **must** insert the script back into the matching cells of the notebook and run the code. Only the notebook will be submitted in Moodle (in `.ipynb` format).
- Please write your answers to questions in red.
- **Important:** All plots, results, and outputs should be included in the notebook as the cells' outputs (run all cells and do not clear the output).
- **Important:** Your submission must be entirely your own. Any attempts of plagiarism (including ChatGPT) will lead to grade 0 and disciplinary actions.

## Question 1 - Bagging
In HW3, you helped Charles Darwin with the regression of the abalone problem and now, you will try combining multiple regression models instead of just one, hopefully for a better result.

### Instructions:
1. Import the necessary libraries.
2. Load the abalone dataset and preprocess it.
3. Implement the `LinRegCombiner` class for bagging with linear regression.
4. Implement the `RidgeLinRegCombiner` class for bagging with ridge regression.
5. Tune the hyperparameters for `RidgeLinRegCombiner` and compare both models.

## Question 2 - Clustering
We learned about partitional clustering and specifically – the K-means algorithm. In this question, you will implement it and see some nice applications.

### Instructions:
1. Implement the `Kmeans` class.
2. Load the exams dataset and plot it.
3. Fit the `Kmeans` model with 2 clusters and visualize the results.
4. Use the Elbow Method to choose the optimal number of clusters between 1-10 and explain your choice.
5. Apply K-means clustering with the selected number of clusters.
6. Compress an image using K-means clustering to reduce the number of colors to 20.

## Question 3 - PCA, LDA
You will try to classify the smiling faces dataset using feature reduction and KNN (since there are 4096 features!). Then, you will compare it to LDA.

### Instructions:
1. Implement PCA to reduce the dimensionality of the images.
2. Apply PCA to the training and test sets.
3. Use the EIG_CDF function to choose the optimal number of dimensions that preserve 95% of the energy.
4. Train a KNN model on the reduced dataset and tune the hyperparameters.
5. Compare the results with LDA.