
# NumPy Basic

## ndarry use


```python
import numpy as np
```


```python
my_arr = np.arange(1000000)
```


```python
my_list = list(range(1000000))
```


```python
%time for _ in range(10): my_arr2 = my_arr * 2
```

    Wall time: 57.6 ms
    


```python
%time for _ in range(10): my_list2 = [x * 2 for x in my_list]
```

    Wall time: 903 ms
    


```python
type(my_arr)
```




    numpy.ndarray




```python
np.random.randn(2,5).shape
```




    (2, 5)




```python
np.empty((2,3,2))
```




    array([[[4.4e-323, 0.0e+000],
            [0.0e+000, 0.0e+000],
            [0.0e+000, 0.0e+000]],
    
           [[0.0e+000, 0.0e+000],
            [0.0e+000, 0.0e+000],
            [0.0e+000, 0.0e+000]]])




```python
sum(np.arange(101))
```




    5050



Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3
