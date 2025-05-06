# EX 1C Quick Sort
## DATE:
## AIM:
To write a python program to implement quick sort using tha last element as pivot on the list of float values.

## Algorithm
1. Select a Pivot: Choose the last element in the list as the pivot.

2. Partitioning: Rearrange the list such that all elements smaller than the pivot are placed before it and all elements greater than the pivot are placed after it. The pivot is now in its correct position.

3. Recursively Sort: Apply the quick sort to the sublist before the pivot and the sublist after the pivot.

4. Base Case: If a sublist has 1 or fewer elements, it is already sorted
## Program:

Developed by: Kishore S
Register Number:  212222240050
```python
def partition(arr,low,high):
    i = ( low-1 )
    pivot = arr[high]
    for j in range(low , high):
        if arr[j] <= pivot:
            i = i+1
            arr[i],arr[j] = arr[j],arr[i]
    arr[i+1],arr[high] = arr[high],arr[i+1]
    return ( i+1 )
def quickSort(arr,low,high):
    if low < high:
        pi = partition(arr,low,high)
        quickSort(arr, low, pi-1)
        quickSort(arr, pi+1, high)
 # Driver code to test above 
arr = []
n = int(input())
for i in range(n):
    arr.append(eval(input()))
quickSort(arr,0,n-1)
print ("Sorted array is:")
for i in range(n):
    print ("%.1f" %arr[i])
```

## Output:
![image](https://github.com/user-attachments/assets/d1ea8528-2467-4770-89f8-0737a46bc094)



## Result:
The program successfully sorts the input array using the QuickSort algorithm, arranging the elements in ascending order.
