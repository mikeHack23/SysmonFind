# SysmonFind

SysmonFind is a Sysmon event search engine, both local and remote, that allows you to analyze or investigate security incidents in real time. Sysmon must be installed on the computer.

# Summary

Application to read sysmon logs, either local or from remote computers, this application searches whatever, based on free searches or Regex searches, what can you do?

* Analyze which process started the communication to a certain IP,
* Search for some IOCs
* Malware analysis
* Search for event IDs and parser the content
* Forensics
* Use of ByPass to use credentials and consult computers in Domain or not

# Images

![SysmonFind](https://github.com/mikeHack23/SysmonFind/assets/32471855/9742341d-fbf5-4ee8-b4d3-2f59a6e26798)

![SysmonFindID](https://github.com/mikeHack23/SysmonFind/assets/32471855/6d237898-2fa6-4786-96d7-7b147afbf7b2)

![SysmonFindRegex](https://github.com/mikeHack23/SysmonFind/assets/32471855/5c2013ca-1d95-4da0-8ed0-071fbf14e9a8)

![SysmonfindQR](https://github.com/mikeHack23/SysmonFind/assets/32471855/94ec05b8-361b-48b5-840e-a0d85761cd57)


## Expresiones Regulares (REGEX) 
Examples:

### Search for events that have an IP address
#### IPV4
```http
\b(?:\d{1,3}\.){3}\d{1,3}\b
```
#### IPV6
```http
\b(?:[A-Fa-f0-9]{1,4}:){7}[A-Fa-f0-9]{1,4}\b
```
### Look up court case numbers
```http
(?<=[A-Za-z]{2}\d{2}-)\d{4,5}-\d{2}\.\d{4}\.\d{1}\.\d{2}\.\d{4}
```
### Files generated with sequence: 0549.exe, 0550.exe, 0560.exe
```http
[0-9][0-9][0-9][0-9]?\.exe
```

