## Warm up 2

Medium warmup string/list problems with loops (solutions available)

### string_times

Given a string and a non-negative int n, return a larger string that is n copies of the original string.

string_times('Hi', 2) → 'HiHi'</br>
string_times('Hi', 3) → 'HiHiHi'</br
string_times('Hi', 1) → 'Hi'

```
def string_times(str, n):
  result = ""
  for i in range(n):
    result = result + str
  return result
```

### front_times

Given a string and a non-negative int n, we'll say that the front of the string is the first 3 chars, or whatever is there if the string is less than length 3. Return n copies of the front;

front_times('Chocolate', 2) → 'ChoCho'</br>
front_times('Chocolate', 3) → 'ChoChoCho'</br>
front_times('Abc', 3) → 'AbcAbcAbc'

```
def front_times(str, n):
  if len(str)<3:
    return str*n
  elif len(str)>=3:
    return str[0:3]*n
```
