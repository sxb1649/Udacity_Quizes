# Udacity_Quizes
Quiz 2
Compute the mean absolute error for the following line and points:

line: y = 1.2x + 2

points: (2, -2), (5, 6), (-4, -4), (-7, 1), (8, 14)

Ans 3.88

Code in python
>>> x = np.array([(2, -2), (5, 6), (-4, -4), (-7, 1), (8, 14)])
>>> x
array([[ 2, -2],
       [ 5,  6],
       [-4, -4],
       [-7,  1],
       [ 8, 14]])
>>> y=1.2*x[:,0]+2
>>> y
array([ 4.4,  8. , -2.8, -6.4, 11.6])
>>> mae = np.mean(np.abs(y-x[:,1]))
>>> mae
3.88

Same for MSE

Compute the mean squared error for the following line and points:

line: y = 1.2x + 2

points: (2, -2), (5, 6), (-4, -4), (-7, 1), (8, 14)

Ans 21.384

x = np.array([(2, -2), (5, 6), (-4, -4), (-7, 1), (8, 14)])
>>> x
array([[ 2, -2],
       [ 5,  6],
       [-4, -4],
       [-7,  1],
       [ 8, 14]])
>>> y=1.2*x[:,0]+2
>>> y

>>> mse = np.mean((y-x[:,1])**2)
>>> mse
21.384000000000004
