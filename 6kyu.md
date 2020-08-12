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


* Find the odd int
* https://www.codewars.com/kata/54da5a58ea159efa38000836/train/python

```python
def find_it(seq):
    for item in seq:
        if seq.count(item) % 2:
            return item
```
