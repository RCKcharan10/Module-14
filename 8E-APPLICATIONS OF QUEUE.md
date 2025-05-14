# Experiment No: 8e - Deleting Element at Front End of Deque Using Built-in Function

## AIM  
To write a Python program to delete an element at the front end of a deque using the collection's built-in function.

## ALGORITHM  
1. Import `deque` from the `collections` module.
2. Initialize an empty deque.
3. Use a loop to append three elements to the deque using `append()`.
4. Delete an element at the front end of the deque using the `popleft()` function.
5. Print the deque after deletion.

## PROGRAM
```python
from collections import deque

d = deque()

for _ in range(3):
    d.append(input().strip())

d.popleft()

print("The deque after deletion is : ")
print(d)

```

### OUTPUT
![image](https://github.com/user-attachments/assets/e69edc51-824f-4752-8894-11408de19b23)


### RESULT
Thus, the Python program to delete an element at the front end of a deque using the collection's built-in function has been implemented and executed successfully.
