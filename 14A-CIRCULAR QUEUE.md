# Experiment No: 14a- Inserting String Values into Circular Queue

## AIM  
To write a Python program using a function to insert string values into a Circular Queue.

## ALGORITHM  
1. Define a class `Queue` that initializes with a limit (size of the queue).
2. Define functions `isempty()` and `isfull()` to check if the queue is empty or full.
3. Define the `enqueue()` function that adds an element to the queue if it is not full.
   - If the queue is full, print "Queue is full".
4. Define the `dequeue()` function that removes an element from the queue if it is not empty.
   - If the queue is empty, print "Queue is empty, nothing to delete".
5. Define the `display()` function to display the elements of the queue.
6. Read the input size of the queue.
7. Insert string values into the queue using the `enqueue()` function.
8. Display the current state of the queue.

## PROGRAM
```python
class Queue:
    def __init__(self, limit):
        self.queue = []
        self.limit = limit
        self.rear, self.front = 0, 0
        
    def isempty(self):
        return len(self.queue) == 0
        
    def isfull(self):
        return len(self.queue) == self.limit
        
    def enqueue(self, item):
        if self.isfull():
            print("Queue is full")
        else:
            if self.front == self.limit:
                self.front = self.rear - 1
            self.queue.insert(self.front, item)
            self.front += 1
            
    def dequeue(self):
        if self.isempty():
            print("Queue is empty, nothing to delete.")
        else:
            if self.rear == self.limit:
                self.rear = 0
            self.queue.pop(self.rear)
            self.rear += 1
        
    def display(self):
        print(self.queue)

size = int(input())
a = Queue(size)
str1 = input()
str2 = input()
str3 = input()

a.enqueue(str1)
a.enqueue(str2)
a.enqueue(str3)

a.display()

```

### OUTPUT
![image](https://github.com/user-attachments/assets/4486e053-3167-470b-bf7e-da818fc5dc7b)


### RESULT
Thus, the Python program to insert string values into a Circular Queue has been implemented and executed successfully.
