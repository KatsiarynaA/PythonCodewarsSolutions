# 8 level of difficulty


* Multiply
* https://www.codewars.com/kata/50654ddff44f800200000004/train/python

```python
def multiply(a, b):
  return a * b
```


* Even or Odd
* https://www.codewars.com/kata/53da3dbb4a5168369a0000fe/train/python

```python
def even_or_odd(number):
    if number % 2:
        return "Odd"
    else:
        return "Even"
```


* Opposite number
* https://www.codewars.com/kata/56dec885c54a926dcd001095/train/python

```python
def opposite(number):
    return -number
```


* Sum of positive
* https://www.codewars.com/kata/5715eaedb436cf5606000381/train/python

```python
def positive_sum(arr):
    sum = 0
    for i in range(len(arr)):
        if arr[i] >= 0:
            sum += arr[i]
    return sum
```


* Return Negative
* https://www.codewars.com/kata/55685cd7ad70877c23000102/train/python

```python
def make_negative(number):
    return -abs(number)
```


* Remove First and Last Character
* https://www.codewars.com/kata/56bc28ad5bdaeb48760009b0/train/python

```python
def remove_char(s):
    return s[1:-1]
```


* Find the smallest integer in the array
* https://www.codewars.com/kata/55a2d7ebe362935a210000b2/train/python

```python
def find_smallest_int(arr):
    return min(arr)
```


* String repeat
* https://www.codewars.com/kata/57a0e5c372292dd76d000d7e/train/python

```python
def repeat_str(repeat, string):
    return string * repeat
```


* No zeros for heros (")
* https://www.codewars.com/kata/570a6a46455d08ff8d001002/train/python

```python
def no_boring_zeros(n):
    if n == 0:
        return 0
    while n % 10 == 0:
        n /= 10
    return n
```


* Draw stairs (")
* https://www.codewars.com/kata/5b4e779c578c6a898e0005c5/train/python

```python
def draw_stairs(n):
    return "\n".join([" " * i + "I" for i in range(n)])
```
