# 7 level of difficulty


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
