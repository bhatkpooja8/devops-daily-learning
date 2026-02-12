Log Reading commands:
tail: to read latest logs
head: see file beginning
wc:count lines
grep: filter the logs in files

logs are never opened in editor in servers

Process control and system health:
kill: stop the process
kill -9 : forcely stop the process
df : disk space
du: folder size
free: memory usage
uptime : system load

PRACTICAL:
Block 1: Log Reading Basics (25 min)
cd /var/log
ls


Read start of file:

head syslog


Read end of file:

tail syslog


Live log (Ctrl + C to stop):

tail -f syslog


Scrollable view:

less syslog

Log Filtering (20 min)
grep error syslog
grep -i fail auth.log 2>/dev/null


Count log lines:

wc -l syslog


Combine power 💥:

grep error syslog | wc -l

Difference b/n tail and tail -f :
tail: will read last few lines and exit
tail -f : will read last few lines and be on listening and real time data 

Use kill -9 only when:

A process is stuck / unresponsive
Normal kill does not work
The process is not shutting down gracefully
