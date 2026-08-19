# Linear Algebra Projects

This repository contains two projects developed for a **Linear Algebra** course.
The projects explore important concepts such as **eigenvalues, eigenvectors, Power Iteration, Eigenfaces, PageRank, and Singular Value Decomposition (SVD)** through computational and visual examples.

---

## Project 1 — Eigen-Everything: From Faces to the Web

This project demonstrates how the same linear algebra concept — the **dominant eigenvector of a matrix** — can be applied to two very different problems:

* **Face Recognition using Eigenfaces**
* **Web Page Ranking using PageRank**

A shared **Power Iteration** algorithm is implemented and reused in both applications.

### Eigenfaces

The Eigenfaces section uses eigenvectors to represent the most important patterns in a collection of face images.

Main concepts include:

* Eigenvalues and eigenvectors
* Covariance matrices
* Power Iteration
* Deflation
* Top-(k) eigenvectors
* Low-rank approximation
* Data centering
* Face representation and recognition

### PageRank

The PageRank section applies the same Power Iteration method to find the dominant eigenvector of the **Google matrix**.

This eigenvector represents the relative importance of web pages.

Main concepts include:

* Google matrix
* Dominant eigenvector
* Power Iteration
* Damping factor
* Convergence
* Eigengap
* Perron–Frobenius theorem

### Main Idea

Although face recognition and web search appear unrelated, mathematically both problems require finding important eigenvectors of large matrices without explicitly performing a complete matrix diagonalization.

---

## Project 2 — Singular Value Decomposition

The second project focuses on understanding **Singular Value Decomposition (SVD)** both algebraically and geometrically.

For a matrix (A):

[
A = U\Sigma V^T
]

SVD decomposes a matrix transformation into three simpler operations.

### Geometric Interpretation

A matrix can be viewed as a transformation machine.

For example, applying a (2 \times 2) matrix to the points of a unit circle can transform the circle into an ellipse.

SVD explains this transformation in three steps:

1. **(V^T) — First Rotation**

   Rotates the original coordinate system to align it with the preferred directions of the transformation.

2. **(\Sigma) — Stretching**

   Stretches or shrinks the space along specific directions.

   The diagonal elements of (\Sigma) are the **singular values**, which determine the lengths of the principal axes of the transformed ellipse.

3. **(U) — Second Rotation**

   Rotates the stretched shape into its final orientation.

### Visualization

The notebook generates points on a unit circle, applies a transformation matrix, and uses SVD to determine the principal directions and singular values of the resulting ellipse.

This provides a visual interpretation of how matrices transform geometric objects and how SVD decomposes those transformations.

The notebook also introduces SVD as a foundation for practical applications such as **image compression**.

---

## Repository Structure

```text
LA-Projects/
│
├── README.md
├── LA-Project1.ipynb
├── LA-Project2/
│   └── ...
└── .gitignore
```

---

## Technologies

* Python
* Jupyter Notebook
* NumPy
* Matplotlib

---

## Running the Projects

Clone the repository:

```bash
git clone https://github.com/sinahkk/LA-Projects.git
```

Open the project directory:

```bash
cd LA-Projects
```

Then open the Jupyter notebooks using **Jupyter Notebook**, **JupyterLab**, or **VS Code** and run the cells in order.

---

## Topics Covered

* Linear Algebra
* Eigenvalues
* Eigenvectors
* Power Iteration
* Eigenfaces
* PageRank
* Covariance Matrices
* Singular Value Decomposition
* Matrix Transformations
* Low-Rank Approximation
* Numerical Linear Algebra

---

## Summary

These projects demonstrate how fundamental linear algebra concepts can be used to solve practical computational problems.

Project 1 connects eigenvectors to **face recognition and web ranking**, while Project 2 develops the geometric intuition behind **Singular Value Decomposition and matrix transformations**.
