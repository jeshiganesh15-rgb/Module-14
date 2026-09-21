# Exp No: 37 Circular Queue
# AIM
To write a Python program with a function to insert float values into a Circular Queue.

# ALGORITHM
Start

Check if the Circular Queue is full
2 If size == max_size, print "Queue is full" and exit the function

3 If the queue is not full:

4 Read the element to be inserted

5 Convert it to float

6 Insert the element at the tail position

7 Update tail using: tail = (tail + 1) % max_size (circular increment) 8 Increment size by 1

End

# PROGRAM
~~~
Reg - 212222060245 Name - Singamala Rakshitha

class Queue: def init(self, size): self.items = [0] * size self.max_size = size self.head, self.tail, self.size = 0, 0, 0

def enqueue(self, item):
    if self.is_list_full():
        self.size==0
        print("Queue is full")
        return
    self.items[self.tail]=item
    self.tail=(self.tail+1)%self.max_size
    self.size+=1
        
def dequeue(self):
    item=self.items[self.head]
    self.head=(self.head+1)%self.max_size
    self.size-=1
    return item
def is_list_full(self):
    if self.size==self.max_size:
        return True
    return False
    

def is_empty(self):
    if self.size==0:
        return True
    return False
size=int(input()) a=Queue(size) str=float(input()) str1=float(input()) str2=float(input()) a.enqueue(str) a.enqueue(str1) a.enqueue(str2) print(a.items)
~~~
# OUTPUT
<img width="645" height="384" alt="image" src="https://github.com/user-attachments/assets/c59a3d3d-408e-4963-ac8f-28a5f79d0a53" />

# RESULT
Thus the Python program with a function to insert float values into a Circular Queue has been implemented and executed successfully
