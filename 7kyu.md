# 7 level of difficulty


* The wheat/rice and chessboard problem (*)
* https://www.codewars.com/kata/5b0d67c1cb35dfa10b0022c7/train/python

```python
def squares_needed(grains):
    count_of_grains = 0
    count_of_square = 0
    grains_in_square = 1
    while count_of_grains < grains:
        count_of_square += 1
        count_of_grains += grains_in_square
        grains_in_square *= 2
    return count_of_square
```


* Halving Sum (*)
* https://www.codewars.com/kata/5a58d46cfd56cb4e8600009d/train/python

```python
def halving_sum(n):
    s = n
    while n != 1:
        n //= 2
        s += n
    return s
```


* Round up to the next multiple of 5 (*)
* https://www.codewars.com/kata/55d1d6d5955ec6365400006d/train/python

```python
def round_to_next5(n):
    while n % 5 != 0:
        n += 1
    return n
```


* Case swapping (*)
* https://www.codewars.com/kata/5590961e6620c0825000008f/train/python

```python
# 1 solution
def swap(string):
    return string.swapcase()

# 2 solution
def swap(string):
    new_string = ""
    for letter in string:
        if letter.isupper():
            new_string += letter.lower()
        else:
            new_string += letter.upper()
    return new_string
```


* Vowel Count
* https://www.codewars.com/kata/54ff3102c1bad923760001f3/train/python

```python
def get_count(inputStr):
    count = 0
    for item in inputStr:
        if item in "aeiouAEIOU":
            count += 1
    return count
```


* Get the Middle Character
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


* Disemvowel Trolls
* https://www.codewars.com/kata/52fba66badcd10859f00097e/train/python

```python
def disemvowel(string):
    new_string = ""
    for item in string:
        if item not in "aeiouAEIOU":
            new_string += item
    return new_string
```


* You're a square!
* https://www.codewars.com/kata/54c27a33fb7da0db0100040e/train/python

```python
def is_square(n):
    return n ** .5 % 1 == 0 if n >= 0 else False
```


* Square Every Digit
* https://www.codewars.com/kata/546e2562b03326a88e000020/train/python

```python
def square_digits(num):
    s = ""
    for item in str(num):
        s += str(int(item) ** 2)
    return int(s)
```


* Highest and Lowest
* https://www.codewars.com/kata/554b4ac871d6813a03000035/train/python

```python
def high_and_low(numbers):
    list = [int(el) for el in numbers.split(" ")]
    return f"{max(list)} {min(list)}"
```
