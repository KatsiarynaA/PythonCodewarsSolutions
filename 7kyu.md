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


* Mumbling
* https://www.codewars.com/kata/5667e8f4e3f572a8f2000039/train/python

```python
# 1 solution
def accum(s):
    new_s = ''
    for i in range(len(s)):
        new_s += s[i].upper() + s[i].lower() * i + "-"
    return new_s[0:len(new_s) - 1]

# 2 solution
def accum(s):
    return '-'.join(el.upper() + el.lower() * i for i, el in enumerate(s))
```


* Shortest Word
* https://www.codewars.com/kata/57cebe1dc6fdc20c57000ac9/train/python

```python
def find_short(s):
    return min([len(el) for el in s.split()])
```


* Exes and Ohs
* https://www.codewars.com/kata/55908aad6620c066bc00002a/train/python

```python
def xo(s):
    return s.lower().count("o") == s.lower().count("x")
```


* Descending Order
* https://www.codewars.com/kata/5467e4d82edf8bbf40000155/train/python

```python
def descending_order(num):
    return int("".join(sorted(str(num), reverse=True)))
```


* Jaden Casing Strings
* https://www.codewars.com/kata/5390bac347d09b7da40006f6/train/python

```python
def to_jaden_case(string):
    return " ".join(el.capitalize() for el in string.split())
```


* Complementary DNA
* https://www.codewars.com/kata/554e4a2f232cdd87d9000038/train/python

```python
keys = {"A": "T", "T": "A", "C": "G", "G": "C"}
def DNA_strand(dna):
    return "".join([keys[value] for value in dna])
```


* List Filtering
* https://www.codewars.com/kata/53dbd5315a3c69eed20002dd/train/python

```python
def filter_list(l):
    return [el for el in l if type(el) == int]
```


* Beginner Series #3 Sum of Numbers
* https://www.codewars.com/kata/55f2b110f61eb01779000053/train/python

```python
def get_sum(a, b):
    return sum(range(min(a, b), max(a, b) + 1))
```


* Isograms
* https://www.codewars.com/kata/54ba84be607a92aa900000f1/train/python

```python
def is_isogram(string):
    return len(set(string.lower())) == len(string)
```


* Sum of two lowest positive integers
* https://www.codewars.com/kata/558fc85d8fd1938afb000014/train/python

```python
def sum_two_smallest_numbers(numbers):
    numbers.sort()
    return numbers[0] + numbers[1]
```


* Growth of a Population
* https://www.codewars.com/kata/563b662a59afc2b5120000c6/train/python

```python
def nb_year(p0, percent, aug, p):
    years = 0
    while p0 < p:
        p0 += p0 * 0.01 * percent + aug
        years += 1
    return years
```


* Is this a triangle?
* https://www.codewars.com/kata/56606694ec01347ce800001b/train/python

```python
def is_triangle(a, b, c):
    return a + b > c and a + c > b and c + b > a
```


* Find the next perfect square!
* https://www.codewars.com/kata/56269eb78ad2e4ced1000013/train/python

```python
import math

def find_next_square(sq):
    if math.sqrt(sq) % 1 == 0:
        return math.pow(math.sqrt(sq) + 1, 2)
    return -1
```


* Number of People in the Bus (")
* https://www.codewars.com/kata/5648b12ce68d9daa6b000099/train/python

```python
def number(bus_stops):
    return sum([el[0] - el[1] for el in bus_stops])
```
