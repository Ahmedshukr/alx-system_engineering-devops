# 0x05. Processes and signals

###  A PID (i.e., process identification number) is an identification number that is automatically assigned to each process when it is created on a Unix-like operating system. A process is an executing (i.e., running) instance of a program. Each process is guaranteed a unique PID, which is always a non-negative integer. 

### 0. Write a Bash script that displays its own PID.
### 1. Write a Bash script that displays a list of currently running processes.
##### Requirements:

 *   Must show all processes, for all users, including those which might not have a TTY
 *   Display in a user-oriented format
 *   Show process hierarchy

### 2. Using your previous exercise command, write a Bash script that displays lines containing the bash word, thus allowing you to easily get the PID of your Bash process.
###### Requirements:

 *   You cannot use pgrep
 *   The third line of your script must be # shellcheck disable=SC2009 (for more info about ignoring shellcheck error here)

### 3. Write a Bash script that displays the PID, along with the process name, of processes whose name contain the word bash.
##### Requirements:

 *   You cannot use ps

### 4. Write a Bash script that displays To infinity and beyond indefinitely.
##### Requirements:

 *   In between each iteration of the loop, add a sleep 2

