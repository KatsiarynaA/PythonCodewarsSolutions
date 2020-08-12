# 6 level of difficulty


* Multiples of 3 or 5
* https://www.codewars.com/kata/514b92a657cdc65150000006/train/python

```python
def solution(number):
    sum = 0 
    for i in range(3, number):
        if i % 3 == 0 or i % 5 == 0:
            sum += i
    return sum
```
