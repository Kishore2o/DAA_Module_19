# EX 1B Merge Sort
## DATE:
## AIM:
To write a python program to sort the first half of the list using merge sort.

## Algorithm
1. Divide the List: Split the given list into two halves.

2. Sort the First Half: Apply the merge sort algorithm to the first half of the list.

3. Leave the Second Half Unchanged: The second half of the list is not modified.

4. Merge the Sorted First Half with the Unsorted Second Half: Merge the sorted first half and the second half back together.

## Program:

Developed by: Kishore S
Register Number: 212222240050
```python
def merge(arr,l,m,r):
    n1 = m - l +1
    n2 = r-m
    left = [0]*(n1)
    right = [0]*(n2)
    for i in range(0,n1):
        left[i] = arr[l+i]
    for j in range(0,n2):
        right[j] = arr[m+1+j]
    i = j = 0
    k = l
    while(i<n1 and j<n2):
        if(left[i] <= right[j]):
            arr[k] = left[i]
            i+=1
        else:
            arr[k] = right[j]
            j+=1
        k+=1
    while(i<n1):
        arr[k] = left[i]
        i+=1
        k+=1
    while(j<n2):
        arr[k] = right[j]
        j+=1
        k+=1
        
def mergesort(arr,l,r):
    if(l<r):
        m=l+(r-l)//2
        mergesort(arr,m+1,r)
        merge(arr,l,m,r)
n = int(input())
l = []
for i in range(n):
    l.append(int(input()))
print("Given array is")
for i in range(n):
    print(l[i],end=" ")
mergesort(l,0,n-1)
print("\n\nSorted array is")
for i in range(n):
    print(l[i],end=" ")  

```

## Output:
![image](https://github.com/user-attachments/assets/a5bb033e-9852-46d8-88af-b20271f69d83)



## Result:
The program successfully sorts the first half of the given array using merge sort. where only the first half is sorted, and the second half remains unchanged.
