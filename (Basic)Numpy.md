## Numpy
### 배열 만들기
```python
list(range(10))
# [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
import numpy as np
np.array([1, 2, 3, 4, 5])
# array([1, 2, 3, 4, 5]
```
```python
np.array([1, 2, 3, 4, 5])
# array([1, 2, 3, 4, 5])
np.array([3, 1.4, 2, 3, 4])
# array([3. , 1.4, 2. , 3. , 4. ])
np.array([[1, 2],
[3, 4]])
# array([[1, 2],
[3, 4]])
np.array([1, 2, 3, 4], dtype='float’)
# array([1., 2., 3., 4.])
```
### 배열 데이터 타입 dtype
+ List와 다르게 array는 단일타입 구성
```python
arr = np.array([1, 2, 3, 4], dtype=float)
arr # array([1., 2., 3., 4.])
arr.dtype
# dtype(‘float64’)
arr.astype(int)
# array([1, 2, 3, 4])
```
### 다양한 배열 만들기
```python
np.zeros(10, dtype=int)
# array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0])
np.ones((3, 5), dtype=float)
# array([[1., 1., 1., 1., 1.],
[1., 1., 1., 1., 1.],
[1., 1., 1., 1., 1.]])
np.arange(0, 20, 2)
# array([ 0, 2, 4, 6, 8, 10, 12, 14, 16, 18])
np.linspace(0, 1, 5)
# array([0. , 0.25, 0.5 , 0.75, 1. ])
```
### 난수로 채워진 배열 만들기
```python
np.random.random((2, 2))
# array([[0.30986539, 0.85863508],
[0.89151021, 0.19304196]])
np.random.normal(0, 1, (2, 2))
# array([[ 0.44050683, 0.04912487],
[-1.67023947, -0.70982067]])
np.random.randint(0, 10, (2, 2))
# array([[3, 9],
[3, 2]]
```
