# Exp.No:38 DEQUE - INSERTION
# AIM
To write a Python program to insert elements at REAR END of deque using a collection built-in function.

# ALGORITHM
Import the deque class from the collections module. Initialize an empty deque.

Start an infinite loop using while True. In each iteration, take input from the user.

If the input is an empty string, break the loop. If the input is not empty, convert it to an integer and append it to the deque.

After the loop ends, append the values 14 and 15 to the deque. Print the message "The deque after appending at right is :".

Print the contents of the deque.

# PROGRAM
~~~
Reg - 212222060245 Name - Singamala Rakshitha

import collections
n1=int(input())
n2=int(input())
n3=int(input())
de=collections.deque([n1,n2,n3])
de.append(14)
de.append(15)
print("The deque after appending at right is :")
print(de)
~~~
# OUTPUT
<img width="1207" height="336" alt="image" src="https://github.com/user-attachments/assets/9f823d1d-2df5-43f8-b9f7-dc8a86e4264c" />

# RESULT
Thus the Python program to insert elements at REAR END of deque using a collection built-in function has been implemented and executed successfully.
