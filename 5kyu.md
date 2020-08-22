# 5 level of difficulty


* Simple Pig Latin
* https://www.codewars.com/kata/520b9d2ad5c005041100000f/train/python

```python
def pig_it(text):
    return " ".join([word[1:] + word[0] + "ay" if word.isalpha() else word for word in text.split()])
```


* Human Readable Time
* https://www.codewars.com/kata/52685f7382004e774f0001f7/train/python

```python
def make_readable(num):
    return "{:02}:{:02}:{:02}".format(num // 3600, num // 60 % 60, num % 60)
```
