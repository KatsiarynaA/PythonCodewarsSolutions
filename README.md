# PythonCodewarsSolutions


* https://www.codewars.com/kata/53da3dbb4a5168369a0000fe/train/python

```python
def even_or_odd(number):
    if number % 2:
        return "Odd"
    else:
        return "Even"
```


* https://www.codewars.com/kata/514b92a657cdc65150000006/train/python

```python
def solution(number):
    sum = 0 
    for i in range(3, number):
        if i % 3 == 0 or i % 5 == 0:
            sum += i
    return sum
```


* https://www.codewars.com/kata/54ff3102c1bad923760001f3/solutions/python

```python
def get_count(inputStr):
    count = 0
    for item in inputStr:
        if item in "aeiouAEIOU":
            count += 1
    return count
```


* https://www.codewars.com/kata/56747fd5cb988479af000028/train/python

```python
def get_middle(s):
    length = len(s)
    x = length // 2
    if length % 2 == 0:
        return s[x - 1] + s[x]
    else:
        return s[x]
```


* https://www.codewars.com/kata/5715eaedb436cf5606000381/train/python

```python
def positive_sum(arr):
    sum = 0
    for i in range(len(arr)):
        if arr[i] >= 0:
            sum += arr[i]
    return sum
```


* https://www.codewars.com/kata/56bc28ad5bdaeb48760009b0/train/python

```python
def remove_char(s):
    return s[1:-1]
```
