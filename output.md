# Vlc Audit - Script Execution Outputs

This document contains simulated terminal outputs for the 5 audit scripts.

---

## 1. System Identity Report (`01-identify.sh`)
```bash
Gaurav@ubuntu-server:~/Vlc$ ./01-identify.sh
================================================================================
                   Vlc AUDIT - SYSTEM IDENTITY                    
================================================================================
Linux Distribution: Ubuntu 22.04.3 LTS
Kernel Version:     5.15.0-89-generic
Current User:       Gaurav
Home Directory:     /home/Gaurav
System Uptime:      up 2 hours, 45 minutes
Current Date/Time:  Mon Mar 30 2026 17:53:09 GMT+0000 (Coordinated Universal Time)
--------------------------------------------------------------------------------
Message: This system runs on Open Source software, providing freedom to study, change, and distribute.
================================================================================
```

---

## 2. FOSS Package Inspector (`02-packages.sh`)
```bash
Gaurav@ubuntu-server:~/Vlc$ ./02-packages.sh
================================================================================
                   Vlc AUDIT - PACKAGE INSPECTOR                 
================================================================================
Status: vlc is INSTALLED on this Ubuntu 22.04.3 LTS system.
Version: 3.0.18-1
--------------------------------------------------------------------------------
FOSS Philosophy Notes:
 - Vlc: A free and open-source media player that promotes the values of open-source software.
 - Firefox: A free and open-source web browser that advocates for a free and open internet.
 - LibreOffice: A free and open-source office suite that supports the open-source movement.
 - GIMP: A free and open-source raster graphics editor that demonstrates the power of community-driven development.
================================================================================
```

---

## 3. Disk and Permission Auditor (`03-auditor.sh`)
```bash
Gaurav@ubuntu-server:~/Vlc$ ./03-auditor.sh
================================================================================
                   Vlc AUDIT - DIRECTORY AUDITOR                 
================================================================================
/etc: Size: 4.0K Permissions: 755 Owner: root
/var/log: Size: 148K Permissions: 755 Owner: root
/usr/bin: Size: 44M Permissions: 755 Owner: root
/usr/lib: Size: 1.4G Permissions: 755 Owner: root
/var/www: Size: 4.0K Permissions: 755 Owner: root
/etc/vlc: Size: 4.0K Permissions: 755 Owner: root
/var/log/vlc: Size: 4.0K Permissions: 755 Owner: root
================================================================================
```

---

## 4. Log File Analyzer (`04-logs.sh`)
```bash
Gaurav@ubuntu-server:~/Vlc$ ./04-logs.sh /var/log/syslog error
================================================================================
                   Vlc AUDIT - LOG FILE ANALYZER                 
================================================================================

Analyzing log file: /var/log/syslog
Searching for keyword: error
Keyword 'error' found 10 times in the log file.
Mar 30 17:45:01 ubuntu-server CRON[1234]: error: failed to execute command
Mar 30 17:46:01 ubuntu-server CRON[1235]: error: failed to execute command
Mar 30 17:47:01 ubuntu-server CRON[1236]: error: failed to execute command
Mar 30 17:48:01 ubuntu-server CRON[1237]: error: failed to execute command
Mar 30 17:49:01 ubuntu-server CRON[1238]: error: failed to execute command
================================================================================
```

---

## 5. Open Source Manifesto Generator (`05-manifesto.sh`)
```bash
Gaurav@ubuntu-server:~/Vlc$ ./05-manifesto.sh
================================================================================
                   Vlc AUDIT - MANIFESTO GENERATOR                 
================================================================================

Please answer the following questions to generate your open-source manifesto:

What is your name? Gaurav
What is your favorite open-source project? Vlc
What do you think is the most important aspect of open-source software? Freedom

My name is Gaurav, and I believe in the power of open-source software. My favorite project is Vlc, which has taught me the importance of collaboration and community-driven development. I think the most important aspect of open-source software is Freedom, as it allows for flexibility and innovation. I will continue to support and contribute to open-source projects, and I hope to inspire others to do the same.

Manifesto generated and saved to Gaurav.txt
================================================================================
```