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


* Sum of Digits / Digital Root
* https://www.codewars.com/kata/541c8630095125aba6000c00/train/python

```python
# 1 solution
def digital_root(n):
    if n > 9:
        sum = 0
        while n != 0:
            sum += n % 10
            n //= 10
        return digital_root(sum)
    else:
        return n

# 2 solution
def digital_root(n):
    return n if n < 10 else digital_root(sum(map(int, str(n))))
```


* Who likes it?
* https://www.codewars.com/kata/5266876b8f4bf2da9b000362/train/python

```python
def likes(names):
    n = len(names)
    formats = {
        0: "no one likes this",
        1: "{} likes this",
        2: "{} and {} like this",
        3: "{}, {} and {} like this",
        4: "{}, {} and {others} others like this"
    }
    return formats[min(n, 4)].format(*names, others = n - 2)
```


* Create Phone Number
* https://www.codewars.com/kata/525f50e3b73515a6db000b83/train/python

```python
# 1 solution
def create_phone_number(n):
    lst = [str(el) for el in n]
    return "(" + "".join(lst[0:3]) + ") " + "".join(lst[3:6]) + "-" + "".join(lst[6:10])

# 2 solution
def create_phone_number(n):
    return "({}{}{}) {}{}{}-{}{}{}{}".format(*n)
```


* Stop gninnipS My sdroW!
* https://www.codewars.com/kata/5264d2b162488dc400000001/train/python

```python
def spin_words(sentence):
    return " ".join([word[::-1] if len(word) >= 5 else word for word in sentence.split()])
```


* Convert string to camel case (")
* https://www.codewars.com/kata/517abf86da9663f1d2000003/train/python

```python
def to_camel_case(text):
    if text == "":
        return ""
    new_text = text[0]
    for i in range(1, len(text)):
        if text[i] == "_" or text[i] == "-":
            new_text += ""
        elif text[i - 1] == "_" or text[i - 1] == "-":
            new_text += text[i].upper()
            i += 1
        else:
            new_text += text[i]
    return new_text
```


* Array.diff (")
* https://www.codewars.com/kata/523f5d21c841566fde000009/train/python

```python
def array_diff(a, b):
    return [num for num in a if num not in b]
```
