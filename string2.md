## String1

Medium python string problems -- 1 loop.. Use + to combine strings, len(str) is the number of chars in a String, str[i:j] extracts the substring starting at index i and running up to but not including index j.

### double_char

Given a string, return a string where for every char in the original, there are two chars.

double_char('The') → 'TThhee'</br>
double_char('AAbb') → 'AAAAbbbb'</br>
double_char('Hi-There') → 'HHii--TThheerree'

```
def double_char(str):
    result = ""
    for i in range(len(str)):
        result = result + str[i]
        result = result + str[i]
        
    return result
```

### count_hi 

Return the number of times that the string "hi" appears anywhere in the given string.

count_hi('abc hi ho') → 1</br>
count_hi('ABChi hi') → 2</br>
count_hi('hihi') → 2

```
def count_hi(str):
  count = 0
  for i in range(len(str)-1):
    if str[i] == 'h' and str[i+1] == 'i':
      count = count + 1
  return count
```

### cat_dog 

Return True if the string "cat" and "dog" appear the same number of times in the given string.

cat_dog('catdog') → True</br>
cat_dog('catcat') → False</br>
cat_dog('1cat1cadodog') → True

```
def cat_dog(str):
  count_cat = 0
  count_dog = 0
  for i in range(len(str)):
    str1 = str[i:i+3]
    if str1 == 'cat':
      count_cat = count_cat + 1
    if str1 == 'dog':
      count_dog = count_dog+1
  return True if (count_dog == count_cat) else False
```
