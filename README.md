# Python-Practice

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
