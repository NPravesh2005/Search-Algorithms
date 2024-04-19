# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```python
#Program to find the element in a list using Binary Search(Iterative Method)..
#Developed by: N.PRAVESH
#RegisterNumber: 212223230154
def binarySearchIter(array, k, low, high):
    while low<=high:
        mid = low + (high - low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low = mid +1
        else:
            high = mid -1
    return -1
    
array = eval(input())
array.sort()
k = eval(input())
result = binarySearchIter(array, k, 0, len(array)-1)
if result==-1:
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ", result)
```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```python
#Program to find the element in a list using Binary Search(Iterative Method)..
#Developed by: N.PRAVESH
#RegisterNumber: 212223230154
def binarySearchIter(array, k, low, high):
    while low<=high:
        mid = low + (high - low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low = mid +1
        else:
            high = mid -1
    return -1
    
array = eval(input())
array.sort()
k = eval(input())
result = binarySearchIter(array, k, 0, len(array)-1)
if result==-1:
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ", result)
```
iii)	# Find the element in a list using Binary Search (recursive Method).
```python
#Program to find the element in a list using Binary Search(Iterative Method)..
#Developed by: N.PRAVESH
#RegisterNumber: 212223230154
def binarySearchIter(array, k, low, high):
    while low<=high:
        mid = low + (high - low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low = mid +1
        else:
            high = mid -1
    return -1
    
array = eval(input())
array.sort()
k = eval(input())
result = binarySearchIter(array, k, 0, len(array)-1)
if result==-1:
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ", result)
```
## Sample Input and Output

(i) Linear search :
![Screenshot 2024-04-19 165858](https://github.com/NPravesh2005/Search-Algorithms/assets/164477756/2dfa94b5-3424-4af6-bb99-85285049cfa2)

(ii) Binary search (Iterative method) :
![Screenshot 2024-04-19 165916](https://github.com/NPravesh2005/Search-Algorithms/assets/164477756/0abed5ba-ef6a-4f70-9035-80b0888558e3)

(iii) Binary search (Recursive method) :
![Screenshot 2024-04-19 165939](https://github.com/NPravesh2005/Search-Algorithms/assets/164477756/d2aa7106-9bc0-4715-9ee4-b83357114fe2)

## Result
Thus the linear search and binary search algorithm is implemented using python programming.
