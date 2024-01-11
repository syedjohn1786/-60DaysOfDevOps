Linux and Shell Scripting
=================================

Linux is an Opensource, Free, Fast and secure Operating system and it has various distributions like Ubuntu, CentOs, Debian.

Kernel is the heart of any Operating System which is responsible for the communication between hardware and software.

Kernel is also responsible for Device management, Memory management, Process Management, handling system calls.

In Linux, Shell is a command-line interface through which we talk/interact with OS by executing commands is called as Shell.

Linux Command :
=====================

ls - list the files and directories

pwd - prints the current working directory

cd - change directory

cd .. - goes back to previous folder (1 step back)

cd ../.. - goes back to 2 previous folders (2 steps back)

ls -ltra = lists the files and directories with size, timestamps, permissions and ownership
( l = permissions, ownership, size, modification time and name)
( t = sorts the list by modification time, latest files will appear first)
( r = reverse the order list)

touch file_name = creates a new text file

mkdir directory_name = creates a new directory

vi file_name = create a new file(if not created) and able to edit the file

cat file_name = prints the content of the file

rm -r directory_name  = removes the directory

free -g = prints the system's memory in gigabytes (it shows total memory, used memory, available memory)

nproc = it shows the no of processors on the system ( shows no of cpu's)

df -h = df stands for disk free and this commands shows the usage of disk space

How can you monitor the CPU, Memory usage ?
Ans : By running "top" command. top command prints the processes that are running , memory usage, disk usage
top = free + nproc + df




