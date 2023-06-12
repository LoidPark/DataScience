## Numpy_3
### Numpy 연산
+ array 기본 연산 지원
```python
x = np.arange(4)
# array([0, 1, 2, 3])
x + 5
# array([5, 6, 7, 8])
x - 5
# array([-5, -4, -3, -2])
x * 5
# array([ 0, 5, 10, 15])
x / 5
# array([0. , 0.2, 0.4, 0.6])
```
### 행렬간 연산
```python
x = np.arange(4).reshape((2, 2))
y = np.random.randint(10, size=(2, 2))
x + y
# array([[1, 7],
[6, 5]])
x - y
# array([[-1, -5],
[-2, 1]])
```
### Broadcasting
+ shape이 달라도 확장되는 형태로 연산이 됨
```python
matrix + 5
matrix + np.array([1, 2, 3])
np.arange(3).reshape((3,1)) + np.arange(3)
```
