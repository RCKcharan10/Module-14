# Experiment No: 8c - Inserting Elements at Rear End of Deque Using Built-in Function

## AIM  
To write a Python program to insert elements 14 and 15 at the rear end of a deque using the collection's built-in function.

## ALGORITHM  
1. Import `deque` from the `collections` module.
2. Initialize an empty deque.
3. Use a loop to append three numbers to the deque using `append()`.
4. Append 14 and 15 to the deque using the `append()` function.
5. Print the deque after appending the elements.

## PROGRAM
```python
from collections import deque

d = deque()

for _ in range(3):
    d.append(int(input()))
    
d.append(14)
d.append(15)

print("The deque after appending at right is : ")
print(d)

```

### OUTPUT
![image](https://github.com/user-attachments/assets/52285cde-4cfd-4b65-b530-873e3883d109)


### RESULT
Thus, the Python program to insert elements 14 and 15 at the rear end of a deque using the collection's built-in function has been implemented and executed successfully.
