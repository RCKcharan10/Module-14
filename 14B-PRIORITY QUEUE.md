# Experiment No: 14b- Simple Implementation of Priority Queue Using Queue

## AIM  
To implement a simple Priority Queue using a Queue and complete the Insert and Delete functions.

## ALGORITHM  
1. Define a class `PriorityQueue` to represent the priority queue.
2. In the constructor `__init__`, initialize an empty queue.
3. Define the `__str__` method to return a string representation of the queue.
4. Define an `isempty()` function to check if the queue is empty.
5. Define the `insert()` function to add an element to the queue.
6. Define the `delete()` function to remove and return the highest priority element (the maximum element).
7. Read input values to insert into the queue.
8. Print the current state of the queue.
9. Continuously delete and print elements from the queue until it is empty.

## PROGRAM
```python
class PriorityQueue(object):
    def __init__(self):
        self.queue = []
        
    def __str__(self):
        return ' '.join([str(i) for i in self.queue])
        
    def isempty(self):
        return len(self.queue) == 0
        
    def insert(self, data):
        self.queue.append(data)
        
    def delete(self):
        try:
            max_val = 0
            for i in range(len(self.queue)):
                if self.queue[i] > self.queue[max_val]:
                    max_val = i
            item = self.queue[max_val]
            del self.queue[max_val]
            return item
        except IndexError:
            print()
            exit()
            
q = PriorityQueue()
n = int(input())
for i in range(0, n):
    ele = int(input())
    q.insert(ele)
print(q)
while not q.isempty():
    print(q.delete())

```

### OUTPUT
![image](https://github.com/user-attachments/assets/1724261d-e1ae-4e98-964a-2bf833fadc1c)

### RESULT
Thus, the Python program for a simple implementation of a Priority Queue using a Queue has been implemented and executed successfully.
