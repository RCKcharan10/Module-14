# Experiment No: 8d - Deleting Element at Rear End of Deque Using Built-in Function

## AIM  
To write a Python program to delete an element at the rear end of a deque using the collection's built-in function.

## ALGORITHM  
1. Import `deque` from the `collections` module.
2. Initialize an empty deque.
3. Use a loop to append three elements to the deque using `append()`.
4. Delete an element at the rear end of the deque using the `pop()` function.
5. Print the deque after deletion.

## PROGRAM
```python
from collections import deque

d = deque()

for _ in range(3):
    d.append(input().strip())
    
d.pop()

print("The deque after deleting at right is : ")
print(d)

```

### OUTPUT
![image](https://github.com/user-attachments/assets/49935aeb-7fce-44d5-8cab-1298b86c37a7)


### RESULT
Thus, the Python program to delete an element at the rear end of a deque using the collection's built-in function has been implemented and executed successfully.
