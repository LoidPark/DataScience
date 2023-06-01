## Numpy
### 배열 만들기
```
list(range(10))
# [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
import numpy as np
np.array([1, 2, 3, 4, 5])
# array([1, 2, 3, 4, 5]
```
```
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
```
arr = np.array([1, 2, 3, 4], dtype=float)
arr # array([1., 2., 3., 4.])
arr.dtype
# dtype(‘float64’)
arr.astype(int)
# array([1, 2, 3, 4])
```
