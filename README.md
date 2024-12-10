# Python_Day16

#NumPy for Engineers
#Activities: Perform Matrix Operations Relevant to Circuit Design
#Here's a basic example of creating and manipulating arrays with NumPy:
import numpy as np

# Creating arrays
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])

# Element-wise operations
sum_array = a + b
diff_array = a - b
prod_array = a * b
div_array = a / b

print("Sum:", sum_array)
print("Difference:", diff_array)
print("Product:", prod_array)
print("Division:", div_array)








#Matrix Operations
#Let's perform some matrix operations relevant to circuit design:
# Creating matrices
A = np.array([[1, 2], [3, 4]])
B = np.array([[5, 6], [7, 8]])

# Matrix addition
matrix_sum = A + B

# Matrix multiplication
matrix_product = np.dot(A, B)

# Transpose of a matrix
matrix_transpose = np.transpose(A)

# Inverse of a matrix (if it exists)
matrix_inverse = np.linalg.inv(A)

print("Matrix Sum:\n", matrix_sum)
print("Matrix Product:\n", matrix_product)
print("Matrix Transpose:\n", matrix_transpose)
print("Matrix Inverse:\n", matrix_inverse)







#Project: Develop a Program to Solve Kirchhoff’s Current Law (KCL) Equations
import numpy as np

# Coefficient matrix A (modified to ensure it's not singular)
A = np.array([[1, -1, -1],
              [-1, 1, 0],
              [0, 1, -1]])

# Constant matrix B
B = np.array([0, 3, 2])

# Solving the linear equations
currents = np.linalg.solve(A, B)

print("Currents I1, I2, and I3:", currents)

