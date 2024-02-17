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
======================================================
ssh => secure shell, shh connects and login to specified hostname securely
Ex: ssh john@172.0.1.0 => john is the username, 172.0.1.0 is the hostname

whoami => if you are logged in with username "john", whoami command prints john on the terminal
who => this command display the information about users who are currently logged into the system ( it displays login name, login device, login date, time)
uname -a => display the information about the OS and kernal running on your machine(uname = unix name)
uptime => The uptime command in Ubuntu Linux is used to display the current time, how long the system has been running, the number of users currently logged into the system.
Ex : $ uptime
 10:25:31 up 12 days, 20:03,  1 user,  load average: 0.00, 0.01, 0.05

 date => display the date
 Ex: $ date
Sat Feb 17 12:05:15 IST 2024
==============================================================
ifconfig => The ifconfig command in Linux is used to configure and display information about network interfaces on the system. However, it is considered deprecated on many modern Linux distributions in favor of the ip command from the iproute2 package. 

ipconfig => similar functionality like ifconfig, but ipconfig is for windows os
Ex: ipconfig

Wireless LAN adapter Wi-Fi:

   Connection-specific DNS Suffix  . :
   Link-local IPv6 Address . . . . . : fe80::ace8:92db:e026:d0f1%15
   IPv4 Address. . . . . . . . . . . : 192.168.1.22
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . : 192.168.1.1

====================================================================
hostname => In Linux, the hostname command is used to view or set the hostname of the system. The hostname is the label assigned to the computer, which typically identifies it within a network. It's often used for system identification and networking purposes.
Ex:
Dell@DESKTOP-VFHMSUF MINGW64 ~
$ hostname
DESKTOP-VFHMSUF
================================================================
free => display amount of free and used memory in the system (The free command displays information about the system's memory usage)
df -h => (disk free) The df command displays information about disk space usage on filesystems. It shows the total disk space, used space, available space, and the percentage of usage for each filesystem mounted on the system. ( C drive, D drive)
$ df -h
Filesystem            Size  Used Avail Use% Mounted on
C:/Program Files/Git  184G  102G   82G  56% /
D:                    293G  230G   64G  79% /d

du -h => (disk usage) The du command (short for "disk usage") is used to estimate file and directory space usage. It calculates the disk space used by files and directories recursively. (in simple, du gives folder/file wise space usage)
$ du -h desktop
12K     desktop/DevOps/Terraform
12K     desktop/DevOps
20K     desktop/Jenkins-Sonarqube/OneNote_RecycleBin
3.2M    desktop/Jenkins-Sonarqube
===========================================================================




