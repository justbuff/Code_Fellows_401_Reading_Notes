# Ethical hacking: Log tampering 101

Ethical hackers need to understand how hackers tamper with logs, as it is a common practice with hackers. Tampering with logs is the equivalent of covering obvious tracks that administrators use to catch hackers. 

There is a four-step process to tampering with logs:

- Disable auditing: if logging is turned off, there will be no trail of evidence. Popular command is "auditpol" whihch disables auditing and shows level of logging set.

- Clearing logs: exampls include clearlogs.exe file, Meterpreter shell, Windows Event Viewer, and the Shred tool in Linux.

- Modifying logs: knowing where the logs are in your target system is crucial for any hacker and a simple text editor can be used to modify logs.

- Erasing command history: if the Shred command above was entered, the retained history of bash commands is found in the file ~/.bash_history.
