# Exp.No:36 APPLICATIONS OF QUEUE
# AIM
To write a Python program to implement CPU Process Scheduling using a queue.

# ALGORITHM
Start the program. Define the function CalculateWaitingTime(at, bt, N).

Initialize a list wt of size N with all values set to 0.

Set wt[0] = 0 for the first process.

Print the table header: "P.No.", "Arrival Time", "Burst Time", "Waiting Time".

Print the values for the first process.

For each process from index 1 to N-1:

Calculate wt[i] = (at[i - 1] + bt[i - 1] + wt[i - 1]) - at[i].

Print the process number, arrival time, burst time, and waiting time.

Initialize total_waiting_time = 0.

Add up all waiting times.

Calculate average waiting time as average = total_waiting_time / N. Print the average waiting time.

Get burst times as input from the user for 5 processes. Call CalculateWaitingTime() with at, bt, and N.

End the program.

# PROGRAM
~~~
Reg - 212222060245 Name - Singamala Rakshitha

	# first process is 0
	wt[0] = 0

	# calculating waiting time
	for i in range(1, n ):
		wt[i] = bt[i - 1] + wt[i - 1]

# Function to calculate turn
# around time
def findTurnAroundTime(processes, n,
					bt, wt, tat):

	# calculating turnaround
	# time by adding bt[i] + wt[i]
	for i in range(n):
		tat[i] = bt[i] + wt[i]

# Function to calculate
# average time
def findavgTime( processes, n, bt):

	wt = [0] * n
	tat = [0] * n
	total_wt = 0
	total_tat = 0

	# Function to find waiting
	# time of all processes
	findWaitingTime(processes, n, bt, wt)

	# Function to find turn around
	# time for all processes
	findTurnAroundTime(processes, n,
					bt, wt, tat)

	# Display processes along
	# with all details
	print( "Processes Burst time " +
				" Waiting time " +
				" Turn around time")

	# Calculate total waiting time
	# and total turn around time
	for i in range(n):
	    total_wt=total_wt+wt[i]
	    total_tat=total_tat+tat[i]
	for i in range(n):
	    print(" "+ str(i+1)  +"   "+str(bt[i])+"  "+str(wt[i])+"    "+str(tat[i]))
	
	print( "Average waiting time = "+
				str(total_wt / n))
	print("Average turn around time = "+
					str(total_tat / n))

# Driver code
if __name__ =="__main__":
	
	# process id's
	processes = [ 1, 2, 3]
	n = len(processes)

	# Burst time of all processes
	t0=int(input())
	t1=int(input())
	t2=int(input())
	burst_time = [t0,t1,t2]

	findavgTime(processes, n, burst_time)
~~~

# OUTPUT
<img width="1189" height="489" alt="image" src="https://github.com/user-attachments/assets/af7cfd2f-34fd-4491-95d6-38348a4dc50f" />

# RESULT
Thus the Python program to implement CPU Process Scheduling using a queue has been implemented and executed successfully.
