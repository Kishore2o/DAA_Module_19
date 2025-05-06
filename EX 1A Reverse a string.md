# EX 1A Reverse a String
## DATE:
## AIM:
To write a program to create a recursive function to reverse a string.

## Algorithm
1. Check the Base Case: If the string is empty or has only one character, return the string as it is.

2. Recursive Step: Take the first character of the string and call the function recursively with the rest of the string.

3. Concatenate: After the recursive call, add the first character to the result of the recursive call.

4. Return the Result: Once the recursion completes, the string will be reversed.  

## Program:
Developed by: Kishore S

Register Number: 212222240050

```python
def revstring(str):
    print(str[::-1])

str=input()
revstring(str)

```

## Output:
![image](https://github.com/user-attachments/assets/ca1a5f88-7fba-4857-b058-0dbba7650e3a)



## Result:
The program successfully reverses the input string using recursion. When the user provides an input string, the output displays the reversed version of the string
