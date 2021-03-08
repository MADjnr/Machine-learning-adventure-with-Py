# Machine-learning-adventure-with-Py
#A Numpy array looks this:
import numpy as np 
x = np.array([[1,2,3], [4,5,6]])
print("x:\n{}".format(x))

from scipy import sparse
#create a 2D Numpy array with a daigonal of ones, and zeros everywhere else
eye = np.eye(4)
print("numpy array:\n{}".format(eye))


#convert the numpy array to a scipy sparse matrix in CSR format
#only thr nonzero entries are stored
sparse_matrix = sparse.csr_matrix(eye)
print("\nscipy sparse CSR matrix:\n{}".format(sparse_matrix))


import matplotlib.pyplot as plt 
#generate a sequence of numbers from -10 t0 10 with 100 in 
x = np.linespace(-10, 10, 100)
#create a second array using sine
y = np.sin(x)
#the plot function makes a line chart of one array against another
plt.plot(x, y, marker = "x")


import pandas as pd 
#create a simple dataset of people
data = {'Name':["john", "Anna", "peter", "Linda"], 
'Location': ["New York", "Paris", "Berlin", "London"], 'Age': [24, 13, 53, 33]
}
data_pandas = pd.DataFrame(data)
 display(data_pandas)

