# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
```
1.Get the array as input
2.Use the array.() function to fine the linear search and binary search
3.print array.
4.print the result.
```




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
```
Program for linear search method to match the item in a list
Developed by:vikash s
RegisterNumber: 22008879
'''
def linearSearch(array,n,k):
    for i in range(0,n):
        if(array[i]==k):
            return i
    return -1
array=eval(input())
k=eval(input())
n=len(array)
array.sort()
result=linearSearch(array,n,k)
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)



```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```

Program to find the element in a list using Binary Search(Iterative Method)..
Developed by:vikash s
RegisterNumber: 22008879
'''
def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
    array = eval(input())
array.sort()
# sort the array
k = eval(input()) 
result=binarySearchIter(array,k,0,len(array)-1)
if (result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)




```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
Program to find the element in a list using Binary Search (recursive Method).
Developed by: vikash s
RegisterNumber: 220088789
'''
def BinarySearch(arr, k, low, high):
    if high>=low:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]>k:
            return BinarySearch(array, k, low, high-1)
        else:
            return BinarySearch(array, k,mid+1,high)
    else:
        return -1

k = eval(input())
result=BinarySearch(array, k,0,len(array)-1)
if (result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)



```
## Sample Input and Output

![Screenshot (88)](https://user-images.githubusercontent.com/119433834/215098039-2bff91e1-25c7-45a4-b72b-d0c2cd36bc1d.png)

![Screenshot (85)](https://user-images.githubusercontent.com/119433834/215098055-74117596-05d0-4fdf-b60c-9c7708704ac3.png)


![Screenshot (86)](https://user-images.githubusercontent.com/119433834/215098073-833f2651-9f74-41d9-b87c-1ea386c14b0d.png)

![Screenshot (87)](https://user-images.githubusercontent.com/119433834/215098097-2bf093a1-0e6c-4f60-8db0-04ec2769b589.png)

## Result
Thus the linear search and binary search algorithm is implemented using python programming.
