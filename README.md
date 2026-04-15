# Machine Learning Fundamentals (Python + Jupyter Notebooks)

## Overview

This repository contains implementations of fundamental machine learning algorithms using Python and Jupyter Notebooks.

It focuses on understanding core ML concepts through step-by-step implementation and experimentation on structured datasets.

---

## Why I Built This

I created this repository to:

* Understand foundational machine learning algorithms
* Implement concept learning and clustering techniques
* Work with real structured datasets in ML workflows

---

## Project Structure

```plaintext id="structure1"
machine-learning-fundamentals/
│── notebooks/
│     ├── candidate_elimination.ipynb
│     ├── kmeans_clustering.ipynb
│     ├── hierarchical_clustering.ipynb
│── data/
│     └── books_data-Final.xlsx   # required dataset for Candidate Elimination
│── requirements.txt
│── README.md
```

---

## Projects Included

### Candidate Elimination Algorithm

Implements the Candidate Elimination algorithm to learn hypotheses consistent with training data using version spaces.

#### Dataset Requirement

This notebook requires the following dataset:

* File: `books_data-Final.xlsx`
* Format: Excel file (.xlsx)
* Columns expected:

  * Title
  * Author
  * Year
  * Language (target label)

#### Note

* The model treats **"English"** as the positive class label
* Other languages are treated as negative examples
* The dataset is loaded using pandas `read_excel()`

---

### K-Means Clustering

Unsupervised learning algorithm used to group data into k clusters based on feature similarity.

---

### Hierarchical Clustering

Agglomerative clustering using linkage methods with dendrogram visualization.

---

## Tech Stack

* Python
* Jupyter Notebook
* pandas
* numpy
* scikit-learn
* matplotlib
* scipy

---

## Dataset Setup (IMPORTANT)

Before running the notebooks:

1. Place the dataset inside the `data/` folder:

   ```plaintext id="dataset1"
   data/books_data-Final.xlsx
   ```

2. Ensure the file path in the notebook matches:

   ```python id="path1"
   file_path = "data/books_data-Final.xlsx"
   ```

---

## How to Run

1. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

2. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

3. Open notebooks from the `notebooks/` folder
