# EX 1D Linear search
## DATE:
## AIM:
To write a python program for a search function with parameter list name and the value to be searched using string values.



## Algorithm
1. Check if the search_value is present in list_name using the "in" operator.
2. If present, return the index of search_value using list_name.index(search_value).
3. If not present, return -1.

## Program:
Developed by: Kishore S
Register Number: 212222240050 

```python
def search(List, n):
    for i in List:
        if i==n:
            print("Found")
            return 0
    print("Not Found")        
            
a=int(input())
List=[]
for i in range(1,a+1):
    c=input()
    List.append(c)
n=input() 

    
```

## Output:

![image](https://github.com/user-attachments/assets/0447cf81-2c4d-4e56-98d8-bb9b19fa5bd3)


## Result:
The program was executed successfully, and it correctly checks if the input element is present in the list, printing "Found" if the element exists or "Not Found" if it does not.
