creation of github acct

Pushing to github:
git push https://bhatkpooja8@github.com/bhatkpooja8/nestjs-backend-project.git main

git push https://bhatkpooja8@github.com/bhatkpooja8/devops-daily-learning.git main
repo created
using nano created this file
Linux Directories:
/:(root)
/etc:[editable text configuration]
/var:[logs/www]
/tmp: temporary files[reboot system, file disappears]

Basic Linux Commands:
| Command | Purpose           |
| ------- | ----------------- |
| `ls`    | list files        |
| `cd`    | change directory  |
| `pwd`   | current directory |
| `grep`  | search text       |
| `awk`   | column-based text |
| `sed`   | replace/edit text |
| `ps`    | process list      |
| `top`   | live process view |
| `chmod` | permissions       |
| `chown` | ownership         |

ls -l
total 8
drwxrwxr-x 2 emb-poojkan emb-poojkan 4096 Feb  5 14:35 day1
drwxrwxr-x 2 emb-poojkan emb-poojkan 4096 Feb  5 14:21 day2
emb-poojkan@EMB-BAN-708:~/Desktop/DEVOPS/Practical/devops-daily-learning$ ls -a
.  ..  day1  day2  .git
emb-poojkan@EMB-BAN-708:~/Desktop/DEVOPS/Practical/devops-daily-learning$ ls -la
total 20
drwxrwxr-x 5 emb-poojkan emb-poojkan 4096 Feb  5 14:21 .
drwxrwxr-x 3 emb-poojkan emb-poojkan 4096 Feb  5 14:16 ..
drwxrwxr-x 2 emb-poojkan emb-poojkan 4096 Feb  5 14:35 day1
drwxrwxr-x 2 emb-poojkan emb-poojkan 4096 Feb  5 14:21 day2
drwxrwxr-x 7 emb-poojkan emb-poojkan 4096 Feb  5 14:21 .git


d: directory
ls -a: gives all the . files which are always hidden
ls -l : list all the files with permission and when modified and all details

ls -la is a combination of ls -l and ls -a

owner
group
others

3 parts

Folder Structure:
cd /var/log
ls
will show the logs which exist , if you want to read from those files , then grep error file_name
grep: finds from file

ps:Processes , current running processes in this terminal
Columns you should know:
Column	Meaning
USER	Process owner
PID	Process ID
%CPU	CPU usage
%MEM	Memory usage
VSZ	Virtual memory
RSS	Actual RAM used
STAT	Process state
COMMAND	Command that started process


| Key | Action             |
| --- | ------------------ |
| `q` | quit               |
| `P` | sort by CPU        |
| `M` | sort by memory     |
| `k` | kill a process     |
| `1` | show per-CPU usage |

In real world, If App is slow

top
Who is eating CPU?
ps aux | sort -nrk 3 | head

Memory leak?
ps aux | sort -nrk 4 | head

Kill a bad process:
kill -9 PID


ps shows processes, ps aux shows all system processes, grep filters them, and top provides real-time monitoring.


Write answers to these (important):

What is /etc used for?
etc:editable configuration can be stored inside etc
Where are logs stored?
/var/logs
Difference between ps and top
ps: which processess are running in terminal
top: processes which are running entire system along with memory utilization , cpu utilization
What does chmod +x do?
execute permission can be given through chmod +x
One command you liked today
ls -la
top
grep command to search the particular word from log files, which is very much essential when we th logs are lengthy


