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
```

Program for linear search method to match the item in a list
Developed by: Subhikshaa M
RegisterNumber: 22001030
def linearSearch(array,n,k):
for i in range(0, n):
if array[i] == k:
return i
return -1
array = eval(input())
# sort the array
k = eval(input()) # k-item to be seared for
# get the length of array and store in the variable n
n = len(array)
array.sort()
result = linearSearch(array, n, k) # use the function for linear search
# use if-else to print sorted array and "Element not found" if the item is not
present in the list otherwise print sorted array and "Element found at index: ",
result
if result == -1:
print(array)
print("Element not found")
else:
print(array)
print("Element found at index: ", result)



```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
Program for linear search method to match the item in a list
Developed by: Subhikshaa M
RegisterNumber: 22001030
def binarySearchIter(array, k, low, high):
# Write your code here to find the middle value and check if the desired item
is above or below the middle value
while low <= high:
mid = low + (high - low)//2
if array[mid] == k:
return mid
elif array[mid] < k:
low = mid + 1
else:
high = mid - 1
return -1
array = eval(input())
# sort the array
array.sort()
k = eval(input()) #k-item to be searched
# use the binary search function to find the item in the list
result = binarySearchIter(array, k, 0, len(array)-1)
# use if-else to print sorted array and "Element not found" if the item is not
present in the list otherwise print sorted array and "Element found at index: ",
result
if result == -1:
print(array)
print("Element not found")
else:
print(array)
print("Element found at index: ", result)




```
iii)	# Find the element in a list using Binary Search (recursive Method).
```

Program for linear search method to match the item in a list
Developed by: Subhikshaa M
RegisterNumber: 22001030
def BinarySearch(arr, k, low, high):
# Write your code here for binary search using recursive method
if high >= low:
mid = low + (high - low)//2
if arr[mid] == k:
return mid
elif arr[mid] > k:
return BinarySearch(arr, k, low, mid-1)
else:
return BinarySearch(arr, k, mid+1, high)
else:
return -1
arr = eval(input())
#sort the array
arr.sort()
k = eval(input()) # k is the element to be searched for
result = BinarySearch(arr, k, 0, len(arr)-1)# use the binary search function to
find the result
# use if-else to print sorted array and "Element not found" if the item is not
present in the list otherwise print sorted array and "Element found at index: ",
result



```
## INPUT FOR LINEAR SEARCH:
![line](https://user-images.githubusercontent.com/118787344/214045832-d78c0d5b-9a9b-44ac-a19a-e00e526620c7.png)


## INPUT FOR BINARY SEARCH USING ITERATIVE METHODE:
![image](https://user-images.githubusercontent.com/118787344/214046001-675b9fc6-2068-40a9-a26b-121072a5614c.png)


## INPUT FOR BINARY SEARCH USING RECURSIVE METHODE :
![image](https://user-images.githubusercontent.com/118787344/214046207-864b79d7-1e9b-4083-8e4d-1afead2510dd.png)

##OUTPUT FOR LINEAR SEARCH:
![image](https://user-images.githubusercontent.com/118787344/214047222-ddd30deb-d496-4569-b0b8-295ff5230bce.png)

##OUTPUT FO BINARY SEARCH USING ITERATIVE METHODE:
![image](https://user-images.githubusercontent.com/118787344/214047700-3834ed62-40e1-48e4-b84f-893b90dc4ea2.png)


##OUTPUT FOR BINARY SEARCH USING RECURSIVE METHODE :
![image](https://user-images.githubusercontent.com/118787344/214047798-12bbe031-2bb6-477a-be4a-49ac498413fc.png)







## Result
Thus the linear search and binary search algorithm is implemented using python programming.
