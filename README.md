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
