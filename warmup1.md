## Warm up1

### sleep_in

The parameter weekday is True if it is a weekday, and the parameter vacation is True if we are on vacation. We sleep in if it is not a weekday or we're on vacation. Return True if we sleep in.


sleep_in(False, False) → True<br/>
sleep_in(True, False) → False<br/>
sleep_in(False, True) → True

```
def sleep_in(weekday, vacation):
  if(weekday):
    return True
  elif(vacation):
    return True
  elif(weekday!=True and vacation !=True):
    return True
  elif(weekday!=True or vacation !=True):
    return False
  else:
    return False
```

### monkey_trouble

We have two monkeys, a and b, and the parameters a_smile and b_smile indicate if each is smiling. We are in trouble if they are both smiling or if neither of them is smiling. Return True if we are in trouble.


monkey_trouble(True, True) → True<br/>
monkey_trouble(False, False) → True<br/>
monkey_trouble(True, False) → False

```
def monkey_trouble(a_smile, b_smile):
  if a_smile== True and b_smile ==True:
    return True
  elif a_smile == False and b_smile == False:
    return True
  else:
    return False
```

### sum_double

Given two int values, return their sum. Unless the two values are the same, then return double their sum.


sum_double(1, 2) → 3<br/>
sum_double(3, 2) → 5<br/>
sum_double(2, 2) → 8

```
def sum_double(a, b):
  if a == b:
    return 2*(a+b)
  else:
    return a+b
```

### diff21

Given an int n, return the absolute difference between n and 21, except return double the absolute difference if n is over 21.


diff21(19) → 2<br/>
diff21(10) → 11<br/>
diff21(21) → 0

```
def diff21(n):
  return (2*(n-21)) if n>21 else 21-n 
```


### parrot_trouble

We have a loud talking parrot. The "hour" parameter is the current hour time in the range 0..23. We are in trouble if the parrot is talking and the hour is before 7 or after 20. Return True if we are in trouble.


parrot_trouble(True, 6) → True<br/>
parrot_trouble(True, 7) → False<br/>
parrot_trouble(False, 6) → False

```
def parrot_trouble(talking, hour):
  return True if (talking and (hour<7 or hour>20)) else False
```

### makes10

Given 2 ints, a and b, return True if one if them is 10 or if their sum is 10.


makes10(9, 10) → True<br/>
makes10(9, 9) → False<br/>
makes10(1, 9) → True

```
def makes10(a, b):
  return True if (a ==10 or b ==10 or a+b == 10) else False
```

### near_hundred

Given an int n, return True if it is within 10 of 100 or 200. Note: abs(num) computes the absolute value of a number.


near_hundred(93) → True<br/>
near_hundred(90) → True<br/>
near_hundred(89) → False

```
def near_hundred(n):
  if (abs(100-n)<=10) or (abs(200-n)<=10) :
    return True
  return False
```

### pos_neg

Given 2 int values, return True if one is negative and one is positive. Except if the parameter "negative" is True, then return True only if both are negative.


pos_neg(1, -1, False) → True<br/>
pos_neg(-1, 1, False) → True<br/>
pos_neg(-4, -5, True) → True

```
def makes10(a, b):
  return True if (a ==10 or b ==10 or a+b == 10) else False
```

### not_string

Given a string, return a new string where "not " has been added to the front. However, if the string already begins with "not", return the string unchanged.


not_string('candy') → 'not candy'<br/>u
not_string('x') → 'not x'<br/>
not_string('not bad') → 'not bad'

```
def not_string(str):
  if str[0:3]!= 'not':
    return ("not"+" "+str)
  else:
    return str
```

### missing_char

Given a non-empty string and an int n, return a new string where the char at index n has been removed. The value of n will be a valid index of a char in the original string (i.e. n will be in the range 0..len(str)-1 inclusive).


missing_char('kitten', 1) → 'ktten'<br/>
missing_char('kitten', 0) → 'itten'<br/>
missing_char('kitten', 4) → 'kittn'

```
def missing_char(str, n):
    return str[0:n]+str[n+1:]
```
   
### front_back

Given a string, return a new string where the first and last chars have been exchanged.


front_back('code') → 'eodc'<br/>
front_back('a') → 'a'<br/>
front_back('ab') → 'ba'

```
def front_back(str):
  if len(str)<=1:
    return str
  return str[-1]+str[1:-1]+str[0]
```

### front3

Given a string, we'll say that the front is the first 3 chars of the string. If the string length is less than 3, the front is whatever is there. Return a new string which is 3 copies of the front.


front3('Java') → 'JavJavJav'<br/>
front3('Chocolate') → 'ChoChoCho'<br/>
front3('abc') → 'abcabcabc'

```
def front3(str):
  if len(str)<3:
    return str*3
  return str[0:3]*3
```
