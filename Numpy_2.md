## Numpy_2
### Indexing
```python
x = np.arange(7)
x[3]
# 3
x[7]
# IndexError: index 7 is out of bounds
x[0] = 10
# array([10, 1, 2, 3, 4, 5, 6])
```
### Slicing
```python
x = np.arange(7)
x[1:4]
# array([1, 2, 3])
x[1:]
# array([1, 2, 3, 4, 5, 6])
x[:4]
# array([0, 1, 2, 3])
x[::2]
array([0, 2, 4, 6]
```
### Reshape
```python
x = np.arange(8)
x.shape
# (8,)
x2 = x.reshape((2, 4))
# array([[0, 1, 2, 3],
[4, 5, 6, 7]])
x2.shape
# (2, 4)
```
### Concatenate
+ axis=0 : 아래로 붙임
```python
x = np.array([0, 1, 2])
y = np.array([3, 4, 5])
np.concatenate([x, y])
# array([0, 1, 2, 3, 4, 5])
```
+ axis=1 : 옆으로 붙임
```python
matrix = np.arange(4).reshape(2, 2)
np.concatenate([matrix, matrix], axis=0)
matrix = np.arange(4).reshape(2, 2)
np.concatenate([matrix, matrix], axis=1)
```
### Split
+ [3], axis=0 : 3번 행 부터 아래위로 나눔
```python
matrix = np.arange(16).reshape(4, 4)
upper, lower = np.split(matrix, [3], axis=0)
```
+ [3], axis=1 : 3번 열 부터 좌우로 나눔
```python
matrix = np.arange(16).reshape(4, 4)
left, right = np.split(matrix, [3], axis=1)
```
