# 7 level of difficulty


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
