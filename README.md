# Optimized Matrix Operations

This repository features optimized C programs for various **matrix manipulation operations**, including **LU Decomposition**, **Matrix Multiplication**, and **Matrix Inversion** using multiple algorithms. The goal of this project is to optimize and improve the performance of matrix operations, which are critical in fields like **scientific computing**, **machine learning**, and **data analysis**.

### Objective:
The purpose of this repository is to demonstrate various algorithms for matrix operations that not only solve common matrix problems, but also improve their performance and computational efficiency. The techniques included in this repository aim to handle large matrices more efficiently than basic, naive approaches. By experimenting with algorithms like **Strassen's Matrix Multiplication** and **LU Decomposition**, this project helps in understanding how different approaches affect the speed and scalability of matrix operations.

## Repository Files

- **LU_decomposition.c**: C implementation of LU Decomposition.
- **LU_inverse.c**: Matrix inversion using LU Decomposition.
- **Naive_matrix_multiplication.c**: C implementation of matrix multiplication using the naive approach.
- **Strassen_multiplication.c**: Matrix multiplication using the Strassen algorithm for better performance.
- **Strassen_inverse_using_naive_multiplication.c**: Matrix inversion using the Strassen algorithm with naive multiplication.
- **Strassen_inverse_using_strassen_multiplication.c**: Matrix inversion using the Strassen algorithm with Strassen multiplication.
- **makefile**: A Makefile to automate compilation and cleaning processes.
- **Report.pdf**: A detailed report explaining the algorithms and implementation details.

## Algorithms Explained

This repository implements several algorithms for matrix manipulation. Each of these algorithms has specific performance benefits for different use cases.

### 1. **LU Decomposition (LU Decomposition Algorithm)**:
LU Decomposition is a method of decomposing a matrix into the product of a lower triangular matrix **L** and an upper triangular matrix **U**. This decomposition is useful in solving systems of linear equations and is a key technique in numerical analysis and computational mathematics.

- **Usage**: Typically used to solve a system of linear equations, calculate determinants, and find matrix inverses more efficiently than direct methods.

### 2. **Naive Matrix Multiplication (Naive Matrix Multiplication Algorithm)**:
The naive matrix multiplication algorithm is the most straightforward approach to multiplying two matrices. It has a time complexity of **O(n³)**, making it inefficient for large matrices.

- **Usage**: This approach is simple to implement but is not recommended for large matrices due to its high computational cost.

### 3. **Strassen's Matrix Multiplication (Strassen Algorithm)**:
Strassen’s algorithm is an optimized method for matrix multiplication that reduces the time complexity to approximately **O(n².81)**. It works by dividing the matrices into smaller sub-matrices and recursively multiplying them using fewer operations compared to the naive approach.

- **Usage**: This algorithm is faster than the naive method and is particularly useful for larger matrices. It’s often used in applications where performance is a concern.

### 4. **Matrix Inversion Using LU Decomposition**:
Matrix inversion using LU Decomposition leverages the fact that if a matrix can be decomposed into **L** and **U**, then its inverse can be computed more efficiently. This method avoids the direct matrix inversion approach, which would otherwise be computationally expensive.

- **Usage**: Commonly used in solving linear systems and inverting matrices when solving problems such as linear regression.

### 5. **Matrix Inversion Using Strassen's Algorithm**:
Strassen's algorithm can also be used to improve the matrix inversion process by first performing matrix multiplication using Strassen's method and then applying inversion.

- **Usage**: Similar to LU Decomposition, Strassen’s inversion method is faster for larger matrices and can be useful when both multiplication and inversion are required.

## Compilation

To compile all the programs, run the following command in your terminal:

```bash
make all
