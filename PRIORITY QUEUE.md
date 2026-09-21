# Exp.No:40 PRIORITY QUEUE
# AIM
To write a Python program for simple implementation of Priority Queue using Queue.

# ALGORITHM
Start the program. Define a class PriorityQueue with an initializer to create an empty list queue.

Define the str method to return queue elements as a string separated by spaces.

Define the isEmpty() method to check if the queue is empty. Define the insert(data) method to append the given data to the queue.

Define the delete() method to: Initialize max_val as 0.

Loop through the queue and find the index of the maximum value. Delete and return the element at that index.

In the main code, take integer input n for number of elements. Loop n times to take input values and insert them into the priority queue. Print the contents of the queue.

While the queue is not empty, call delete() and print each returned element. End the program.

# PROGRAM
~~~
Reg - 212222060245 Name - Singamala Rakshitha

# A simple implementation of Priority Queue
# using Queue.
class PriorityQueue(object):
	def __init__(self):
		self.queue = []

	def __str__(self):
		return ' '.join([str(i) for i in self.queue])

	# for checking if the queue is empty
	def isEmpty(self):
		return len(self.queue) == 0

	# for inserting an element in the queue
	def insert(self, data):
		self.queue.append(data)

	# for popping an element based on Priority
	def delete(self):
	    try:
	        max_val=0
	        for i in range(len(self.queue)):
	            if self.queue[i]>self.queue[max_val]:
	                max_val = i
	        item = self.queue[max_val]
	        del self.queue[max_val]
	        return item
	    except IndexError:
	        print()
	        exit()
	   

myQueue = PriorityQueue()
n=int(input())	
for i in range(0, n):
    ele = int(input())
    myQueue.insert(ele)
	
print(myQueue)		
while not myQueue.isEmpty():
	print(myQueue.delete())
~~~
# OUTPUT
<img width="1195" height="452" alt="image" src="https://github.com/user-attachments/assets/a46e5e77-19ac-4043-87f7-4b6f6862e828" />

# RESULT
Thus the Python program for simple implementation of Priority Queue using Queue has been implemented and executed successfully.
