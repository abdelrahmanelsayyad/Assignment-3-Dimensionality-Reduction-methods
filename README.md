# Assignment #3: Dimensionality Reduction Methods

**Course**: AIE425 Intelligent Recommender Systems, Fall Semester 24/25  
**Assignment**: #3 (10% of the course mark)  
**Student ID**: A20001136  
**Name**: Abdelrahman El-Sayyad  
**Due Date**: December 31, 2024 (Week 14 Lab)

---

## Overview

This repository contains all **code** and the **report** for **Assignment #3**, which explores **dimensionality reduction** for recommendation systems. Specifically, we demonstrate:

1. **PCA Method with Mean-Filling**  
2. **PCA Method with Maximum Likelihood Estimation (MLE)**  
3. **Singular Value Decomposition (SVD)**  

Each method focuses on predicting **missing ratings** in a user–item dataset. We identify two **lowest-rated items** (I1 and I2) and compare the approaches in terms of predictions, accuracy, and pros/cons.

---

## Repository Structure

├── code │ ├── assignment3_pca_meanfill.py # Part 1 (PCA + Mean-Filling) │ ├── assignment3_pca_mle.py # Part 2 (PCA + MLE) │ ├── assignment3_svd.py # Part 3 (SVD) │ └── additional_helpers.py # (if any helper scripts) ├── data │ └── modified_dataset.csv # The dataset from Assignments #1/#2 ├── report │ └── assignment3_report.pdf # Final write-up and discussion ├── README.md # This file (overview & usage)


---

## How to Run

1. **Clone or download** this repository.
2. Make sure you have **Python 3.x** and the necessary libraries installed:
   - `numpy`
   - `pandas`
   - `matplotlib`
   - (optionally `jupyter` if you prefer running notebooks)
3. **Navigate** to the `code` folder in your terminal or IDE.
4. Run each script (e.g., `python assignment3_pca_meanfill.py`) to see the console output:
   - **Part 1**: `assignment3_pca_meanfill.py`
   - **Part 2**: `assignment3_pca_mle.py`
   - **Part 3**: `assignment3_svd.py`
5. Check the **console** for printed outputs (e.g., covariance matrices, missing rating predictions, comparisons).
6. The **report** (in `report/assignment3_report.pdf`) includes a written summary, methodology, and conclusions.

---

## Key Results

- **Part 1** (Mean-Filling PCA)  
  Identifies top-5 and top-10 peer items for each target, uses a simple average for predictions.

- **Part 2** (MLE PCA)  
  Computes covariance only over overlapping ratings, potentially more accurate in some cases.

- **Part 3** (SVD)  
  Decomposes the entire matrix (with global mean-filling) into latent factors, then reconstructs missing ratings.

---

## References & Notes

- The **dataset** (`modified_dataset.csv`) originates from **Assignment #1/#2**, already scaled to a **1–5** rating range.
- Detailed instructions are found in the assignment specification.  

---

## Contact

For any questions regarding the code or the assignment:
- **Name**: Abdelrahman El-Sayyad
- **Email**: *Abdoelsayyad@gmail.com*

Please **open an issue** on this GitHub repo if you encounter any problems running the code.
