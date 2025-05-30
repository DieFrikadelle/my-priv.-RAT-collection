# **NonEuclid** 
![NonEuclid-RAT-3](https://github.com/user-attachments/assets/1ba16b3b-29a7-4e01-8f2e-6816394c60fc)

“NonEuclid, developed in C#, is a highly advanced malware that provides unauthorized remote access and employs sophisticated evasion techniques,” Cyfirma stated in a technical analysis published last week.

The RAT leverages a range of methods, including antivirus bypassing, privilege escalation, anti-detection mechanisms, and ransomware encryption targeting critical files.


## Core Functionality
NonEuclid initiates with a client application setup, followed by multiple anti-detection checks. Once these are completed, it establishes a TCP socket for communication with a designated IP address and port. The malware configures exclusions in Microsoft Defender Antivirus to evade detection and monitors processes such as “taskmgr.exe,” “processhacker.exe,” and “procexp.exe,” which are commonly used for process management and analysis.

![Untitled-design-2](https://github.com/user-attachments/assets/c6b0dc5e-c5e3-4f7c-8c2a-cc7ba074c63f)



“NonEuclid employs Windows API calls, such as CreateToolhelp32Snapshot, Process32First, and Process32Next, to enumerate active processes and match their names against specific targets,” Cyfirma noted. Based on the AntiProcessMode setting, it can either terminate these processes or cause the client application to ex.


## Anti-Analysis and Evasion Techniques
The malware incorporates several anti-analysis strategies, including checks to detect virtual machines or sandboxed environments, terminating itself if such conditions are identified. It also bypasses the Windows Antimalware Scan Interface (AMSI) to avoid being flagged by security systems.

![image-16](https://github.com/user-attachments/assets/e48734f8-7012-4e2a-bf12-90015331f2f6)



## Persistence and Ransomware Features
NonEuclid maintains persistence through scheduled tasks and modifications to the Windows Registry. It also attempts to elevate privileges by bypassing User Account Control (UAC) protections to execute commands. Notably, it includes a ransomware component, encrypting files with extensions like .CSV, .TXT, and .PHP and appending them with the extension .NonEuclid.
