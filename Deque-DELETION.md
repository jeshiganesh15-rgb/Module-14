# Exp.No:39 Deque - DELETION
# AIM
To write a Python program to delete elements at FRONT END of deque using a collection built-in function.

# ALGORITHM
Import the deque class from the collections module. Create an empty deque.

Define how many elements to input (e.g., 3 inputs as in the example). Loop through the range of input size:

Read an integer from the user. Append the integer to the deque.

Remove the front element of the deque using popleft(). Print the final deque after deletion.

# PROGRAM
~~~
Reg - 212222060245 Name - Singamala Rakshitha

import collections
  
n1=int(input())
n2=int(input())
n3=int(input())
# initializing deque
de = collections.deque([n1,n2,n3])
de.popleft()
# printing modified deque
print ("The deque after deleting is : ")
print (de)
~~~
# OUTPUT
<img width="1182" height="338" alt="image" src="https://github.com/user-attachments/assets/a1b9a418-5663-43e3-80a5-b95b0bdc32d3" />

# RESULT
Thus the Python program to delete elements at FRONT END of deque using a collection built-in function has been implemented and executed successfully.
