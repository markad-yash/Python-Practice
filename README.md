# Python-Practice

https://www.geeksforgeeks.org/python-list-exercise/

Problem 1:
Python program to interchange first and last elements in a list
```python
lst = [int(i) for i in input().split(' ')]
print(lst)
#swaping the first aand last element form the list
lst[0],lst[-1]=lst[-1],lst[0]
print(lst)
```
OR

```python
lst = [int(i) for i in input().split(' ')]
print(lst)
#swaping the first aand last element form the list
fst = lst[0]
lt  = lst[len(lst)-1]
lst[0]=lt
lst[len(lst)-1]=fst
print(lst)
```

Output:
```
0 1 2 3 4 5 6 7 8 9
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
[9, 1, 2, 3, 4, 5, 6, 7, 8, 0]
```


Problem 2:
Python program to swap two elements in a list

```python
def swap(lst,pos1,pos2):
    lst[pos1],lst[pos2]=lst[pos2],lst[pos1]
    print(lst)

if __name__ =='__main__':
    lst = [i for i in range(1,10)]
    pos1= 2 #element 3 swap with  8
    pos2= 7 #element 8 swap with 3
    print(lst)
    swap(lst,pos1,pos2)
```

Output:
```
[1, 2, 3, 4, 5, 6, 7, 8, 9]
[1, 2, 8, 4, 5, 6, 7, 3, 9]

```

Problem 3: Finding length of list without built-in len() function
```python
lst = [2,3,4,5,8]

size = 0
for i in lst:
    size+=1
    
print('without len()>'size)
print('with len()   >'len(lst))

```
Output:
```
without len()> 5
with len()   > 5
```

Problem 4 : Finding minimum and maximum number in list without using in-build min and max function
```python
lst = [3,2,50,25,7]
lst.sort()
print('sorted list >',lst)
max_num = lst[-1]
min_num = lst[0]
print('maximum number in list > {0}'.format(max_num))
print(f'minimun number in list > {min_num}')
```
Output:
```
sorted list > [2, 3, 7, 25, 50]
maximum number in list > 50
minimun number in list > 2
```
Problem :Python | Ways to check if element exists in list
```python
lst = [3,4,1,56,5,2]

x = lst.count(5)
y = lst.count(20)
print(x)
print(y)
```
Output:
```
1  #1 for True
0  #0 for false
```
Problem :Different ways to clear a list in Python
```python
lst = [i for i in range(10)]
print(lst)
lst.clear()
print(lst)

#OR

for i in range(len(lst)):
    lst.pop()
print(lst)

#OR

lst *=0
print(lst)
```
Output:
```
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
[]
```
Problem :Reverse the list 
```python
lst = [i for i in range(10)]

print(lst)
print(lst[::-1])

#OR

def reverse(lst):
    print([ele for ele in reversed(lst)])

reverse(lst)
```
Output:
```
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
[9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
```
Problem : Python | Cloning or Copying a list
```python
lst = [ele for ele in range(10)]
print(lst)

lst_ =  lst
print(lst_)

#OR

ls = []
for i in lst:
    ls.append(i)
print(ls)

#OR

ls1 = []
ls1.extend(lst)
print(ls1)
```
Output:
```
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```
Problem :Find sum of List in Python
```python

import random

sum =0
lst = []
for i in range(10):
    j = random.randint(1,10)
    sum = sum +j
    lst.append(j)
print(lst)
print(sum)

```
Output:
```
[2, 7, 10, 7, 1, 4, 6, 8, 1, 10]
56
```
Problem : Creating the random number list
```python
import random

lst = []
for i in range(10):
    j = random.randint(1,10)
    lst.append(j)
print(lst)
```
Output:
```
[6, 5, 7, 2, 4, 5, 8, 1, 8, 5]
```
Problem : Multiply all element in list
```python

lst = [6, 5, 7, 2, 4, 5, 8, 1, 8, 5]

mul = 1
for i in lst:
    mul = i*mul
    print(mul)

print(f'Total multiplication of list element is {mul}')

```
Output:
```
6
30
210
420
1680
8400
67200
67200
537600
2688000
Total multiplication of list element is 2688000
```
Problem : Sum of nested list element in list
```python
lst = [[2,1,3],[4,6,3],[5,3,2]]

ls = []

for i in lst:
    count =0
    for j in i:
        count +=j
    ls.append(count)

print(ls)
```
Output:
```
[6, 13, 10]
```
Problem :
```python

```
Output:
```

```
Problem :
```python

```
Output:
```

```
