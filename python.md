## Warm up1

### sleep_in

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

```
def sum_double(a, b):
  if a == b:
    return 2*(a+b)
  else:
    return a+b
```

### diff21

```
def diff21(n):
  return (2*(n-21)) if n>21 else 21-n 
```


### parrot_trouble

```
def parrot_trouble(talking, hour):
  return True if (talking and (hour<7 or hour>20)) else False
```

### makes10

```
def makes10(a, b):
  return True if (a ==10 or b ==10 or a+b == 10) else False
```


### pos_neg

```
def makes10(a, b):
  return True if (a ==10 or b ==10 or a+b == 10) else False
```

### not_string

```
def not_string(str):
  if str[0:3]!= 'not':
    return ("not"+" "+str)
  else:
    return str
```


### front_back

```
def front_back(str):
  if len(str)<=1:
    return str
  return str[-1]+str[1:-1]+str[0]
```

### front3

```
def front3(str):
  if len(str)<3:
    return str*3
  return str[0:3]*3
```
