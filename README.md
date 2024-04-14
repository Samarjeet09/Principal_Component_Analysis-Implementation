# Principal Component Analysis (PCA)
<br>[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Samarjeet09/Principal_Component_Analysis-Implementation/blob/main/Principal_Component_Analysis.ipynb)
## Overview

Principal Component Analysis (PCA) is a dimensionality reduction technique commonly used in data analysis and machine learning. Its primary objective is to identify patterns and relationships in high-dimensional data by transforming it into a lower-dimensional space while preserving the essential information. PCA achieves this by identifying the principal components, which are the orthogonal directions of maximum variance in the data.

## Math Behind PCA

1. **Centering the Data**: PCA begins by centering the data, i.e., subtracting the mean of each feature from the dataset. This step ensures that the data is centered around the origin.

2. **Computing the Covariance Matrix**: Next, PCA computes the covariance matrix of the centered data. The covariance between two variables measures how they vary together. The covariance matrix provides information about the relationships between different features.

3. **Eigenvalue Decomposition**: PCA then performs eigenvalue decomposition on the covariance matrix to find its eigenvectors and eigenvalues. Eigenvectors represent the directions of maximum variance in the data, while eigenvalues indicate the magnitude of variance along these directions.

4. **Selecting Principal Components**: The eigenvectors with the highest eigenvalues (principal components) capture the most variance in the data. Typically, these are sorted in descending order of eigenvalues.

5. **Projecting Data onto Principal Components**: Finally, PCA projects the original data onto the selected principal components, effectively transforming it into a lower-dimensional space.

## How to Perform PCA Without Libraries

### Step 1: Prepare Data

Assuming you have your dataset loaded into a numpy array `X`.

### Step 2: Center the Data

Subtract the mean of each feature from the dataset.

### Step 3: Compute the Covariance Matrix

Calculate the covariance matrix of the centered data.

### Step 4: Perform Eigenvalue Decomposition

Perform eigenvalue decomposition on the covariance matrix to find its eigenvectors and eigenvalues.

### Step 5: Select Principal Components

Sort the eigenvectors by their corresponding eigenvalues in descending order to select the principal components.

### Step 6: Project Data onto Principal Components

Project the original data onto the selected principal components to transform it into a lower-dimensional space.

## Conclusion

PCA is a powerful technique for reducing the dimensionality of data while retaining most of its information. By understanding the underlying mathematics and following the steps outlined above, you can effectively apply PCA without using libraries.
