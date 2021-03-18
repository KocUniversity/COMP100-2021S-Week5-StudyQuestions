1. Write a function that takes a tuple as input and returns a tuple such that each element is incremented by 1.
First do it by converting it to a list and back, then do it without converting to a list and back. 
`increment_tuple((10,20,30))`
> (11,21,31)

2. Write a function that takes a list of tuples as input and replaces the last element of each tuple with the first element of that tuple. ** (You should not convert tuples to list). **
`replace_last([(1, 2, 3), (10, 20), (40, 50, 200, 300)])`
> [(1, 2, 1), (10, 10), (40, 50, 200, 40)]

3. Write a function that takes a nested list and reverses every other list in the main list starting with the first one. (Do not return a new list. Only modify the original list)
```
nested_list = [[1, 2], [3, 4, 5], [6, 7, 8, 9], [10, 11, 12, 13], [14, 15], [16, 17]]
reverse_every_other(nested_list)
print(nested_list)
```
> [[2, 1], [3, 4, 5], [9, 8, 7, 6], [10, 11, 12, 13], [15, 14], [16, 17]]

4. Write a function that takes a tuple as an input and **without converting it to a list and back** returns a tuple with the maximum element removed. (you can assume that the tuple has only 1 maximum element)
`remove_max_from_tuple((100, 20, 300, 15, 48))`
> (100, 20, 15, 48)

5. Write a function that takes a list of lists as an input and returns a simple flat list. (Do not modify the original list. return a new list)
`flatten_list([[10, 20, 30], [40, 50], [60, 70], [80, 90], [100, 110], [120, 130, 140]])`
> [10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120, 130, 140] 

6. Given a list of integers, remove all the elements if the sum of that element and the index of that element is divisibly by 3.
```
l = [15,12,18,21,23,36,39]
# TODO: Your Code Here
print(l)
```
> [12, 18, 36]

7. Assume that `num_list` is a list of numbers. after performing which of the following operations, will `num_list` be different than the others?

A: 
```
for index, item in enumerate(num_list):
   num_list[index] = num_list[index] + 1
```
B:
```
for index, item in enumerate(num_list):
   num_list[index] = item + 1
```
C:
```
for index in range(len(num_list)):
   num_list[index] = num_list[index] + 1
```
D:
```
for item in num_list:
   item += 1
```

8. What will `a`, `b`, `c` be after the following operations?
```
a = [1,2,3]
b = [4,5,6]
c = a
a = b
a.append(20)
```

9. Consider the following functions:
```
def double_first1(a):
    a[0] *= 2
    return a

def double_first2(a):
    a[0] *= 2

def change_list1(a):
    a = [100, 200, 300]
    return a

def change_list2(a):
    a = [1000, 2000, 3000]
```
what will `l1`, `l2`, and `l3` be after the following operations?
```
l1 = [10,20,30]
l2 = double_first1(l1)
double_first2(l2)
l3 = change_list1(l1)
change_list2(l2)