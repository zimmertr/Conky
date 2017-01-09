# Conky

## Summary  

This is a Conky configuration file that was used for years to monitor my Linux desktop before I switched to i3wm and stopped using Conky. The monitor applet shows a lot of useful information pertaining to your system in an easy-to-read, color coded, and rapidly upated way.

Core system metrics are displayed in the first section, The second section is devoted to a To Do list which is simply the results of a text file and $cat. The third section is devoted to displaying your top running processes. 

The applet also takes advantage of a small python script that I wrote that queries the Gmail API for the current number of unread emails on your account. To make this script work, simply insert your email address and password in the script where you see the `user='email'` and `passwd='password'` fields. 

The conky.conf file should be dropped wherever the Conky package looks for the config file on your OS. (Typicall /etc/conky/conky.conf)

The Gmail.py and Todo.txt files should be located in a place where the user running Conky has permissions to read.

![Alt text](https://raw.githubusercontent.com/zimmertr/Conky-Configuration/master/screenshot.png "Screenshot of Conky.")


##Detailed breakdown of all Metrics:

###System Information  
- CPU  
    Usage in GHz  
    Usage in percent  
    Usage as a graph  

- Memory  
    Usage in MiB  
    Usage in percent  
    Usage as a graph  

- HDD  
    Usage in GiB  
    Usage in Percent  
    Usage as a graph  

- Uptime  
    Time since last boot as Hours, Minutes, and Seconds  

- Network
    Current upload speed in b, kb, and mb  
    Current download speed in b, kb, and mb  

- Updates  
    Number of current updates available for your OS  

- Emails  
    Number of unread emails in your GMail account  

- Weather  
    Outside temperature in F  
    Current weather condition  


###To Do List  

First 10 lines of a text file stored on your hard disk. Updates every 1 second.  


###Running Processes  

- Number of current running Processes  

- Top 10 processes in order of CPU Usage  

- Process ID for each process  

- CPU Usage for each process  

- Memory usage for each process  
