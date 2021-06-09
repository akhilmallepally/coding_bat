## List 2

Medium python list problems -- 1 loop.. Use a[0], a[1], ... to access elements in a list, len(a) is the length.

### count_evens 

Return the number of even ints in the given array. Note: the % "mod" operator computes the remainder, e.g. 5 % 2 is 1.

count_evens([2, 1, 2, 3, 4]) → 3</br>
count_evens([2, 2, 0]) → 3</br>
count_evens([1, 3, 5]) → 0</br>

```
def count_evens(nums):
  count = 0
  for i in nums:
    if i %2 ==0:
      count = count+1
  return count
```
