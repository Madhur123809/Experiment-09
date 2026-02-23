# Experiment-09

Madhur Gupta 
25070123070

Experiment No. 9 – Study of NumPy Library
Aim


To study and implement the NumPy (Numerical Python) library in Python by exploring its array creation methods, array attributes, built-in functions, and mathematical operations on arrays.



Theory

Introduction to NumPy:

NumPy, which stands for Numerical Python, is a fundamental open-source library used for scientific and numerical computing in Python. It was created by Travis Oliphant in 2005 and has since become one of the most widely used libraries in the Python ecosystem. NumPy provides support for powerful N-dimensional array objects, sophisticated functions, tools for integrating C and C++ code, and useful linear algebra and random number capabilities. It serves as the backbone for many other popular Python libraries such as Pandas, Matplotlib, SciPy, and Scikit-learn.

Why Use NumPy Over Python Lists?


Python lists, while flexible and easy to use, are not well suited for large-scale numerical computations. NumPy overcomes the limitations of Python lists in several important ways. First, NumPy arrays are stored in contiguous memory blocks, unlike Python lists which store references to objects scattered in memory. This makes data access and manipulation significantly faster. Second, NumPy uses fixed data types for all elements in an array, which eliminates the overhead of type checking that Python lists require for each element. Third, NumPy supports vectorized operations, meaning mathematical operations are applied to entire arrays at once without the need for explicit Python loops. This leads to cleaner, more readable code and much faster execution. Fourth, NumPy arrays consume less memory compared to Python lists for the same amount of data. These combined advantages make NumPy the preferred choice for any task involving numerical data processing, matrix operations, statistical analysis, or scientific computation.

NumPy Array (ndarray):



The core data structure in NumPy is the ndarray, which stands for n-dimensional array. An ndarray is a grid of values, all of the same type, indexed by a tuple of non-negative integers. The number of dimensions is called the rank of the array, and the shape of an array is a tuple of integers giving the size of the array along each dimension. Unlike Python lists, NumPy arrays cannot hold elements of different data types in the same array. This homogeneity is what makes NumPy arrays so efficient for numerical computation. Arrays can be created from Python lists or tuples using the np.array() function.

Array Attributes:



NumPy provides several important attributes that give information about the structure and content of an array. The ndim attribute returns the number of dimensions or axes of the array. For a one-dimensional array it returns 1, and for a two-dimensional array it returns 2. The shape attribute returns a tuple representing the size of the array along each dimension. For example, a 2D array with 2 rows and 3 columns would have a shape of (2, 3). The size attribute returns the total number of elements present in the array, which is the product of the elements of the shape. The dtype attribute returns the data type of the elements stored in the array, such as int64, float64, or bool. Understanding these attributes is essential for correctly manipulating and passing arrays to functions.

Array Creation Functions:



NumPy offers a rich set of built-in functions for creating arrays without manually entering values. The np.zeros() function creates an array of a specified shape filled entirely with zeros, and by default the elements are of type float64. The np.ones() function similarly creates an array filled with ones, and accepts an optional dtype argument to specify the data type. The np.eye() function creates a 2D identity matrix, where all diagonal elements are 1 and all off-diagonal elements are 0. This is frequently used in linear algebra operations. The np.arange() function works similarly to Python's built-in range() function and generates an array of evenly spaced values within a given interval, accepting start, stop, and step arguments. The np.linspace() function generates a specified number of evenly spaced values between a start and end point, making it particularly useful for generating data for plotting and mathematical functions.

Mathematical and Statistical Operations:



One of NumPy's greatest strengths is its ability to perform mathematical and statistical operations on entire arrays efficiently. Basic arithmetic operations such as addition, subtraction, multiplication, and division are applied element-wise when performed on NumPy arrays, meaning the operation is applied to each corresponding pair of elements. This is called broadcasting, and it eliminates the need for writing loops to process each element individually. For example, multiplying an array by 2 doubles every element in the array simultaneously. NumPy also provides dedicated functions for statistical analysis. The np.mean() function calculates the arithmetic mean of all elements in an array. The np.sum() function returns the sum of all elements. Other commonly used functions include np.min(), np.max(), np.std() for standard deviation, and np.median() for the median value. These functions can also operate along a specific axis of a multi-dimensional array, giving row-wise or column-wise results.

Applications of NumPy:



NumPy is used across a wide range of domains including data science, machine learning, image processing, signal processing, and scientific research. In machine learning, NumPy arrays are used 
to represent datasets, weight matrices, and feature vectors. In image processing, images are represented as multi-dimensional NumPy arrays where each pixel value corresponds to an element in the array. In signal processing, NumPy provides tools for Fourier transforms and filtering. Its versatility, performance, and ease of integration with other libraries make it an indispensable tool for anyone working with data in Python.

Conclusion


In this experiment, we successfully studied and implemented the NumPy library in Python. We understood the fundamental reasons for using NumPy over traditional Python lists, primarily due to 
its superior speed, memory efficiency, and support for vectorized operations. We created both one-dimensional and two-dimensional arrays using the np.array() function and examined their properties using built-in attributes such as ndim, shape, size, and dtype. We explored various array creation functions including np.zeros(), np.ones(), np.eye(), np.arange(), and np.linspace(), each of which serves a specific and useful purpose in numerical computing. We also performed element-wise arithmetic operations directly on arrays and applied statistical functions such as np.mean() and np.sum() to compute aggregate values efficiently. Through this experiment, it is evident that NumPy is an essential and powerful library that forms the foundation of data science and scientific computing in Python, and a strong understanding of its features is crucial for any work involving numerical data.


