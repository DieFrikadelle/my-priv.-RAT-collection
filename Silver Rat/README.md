# **Silver Rat**

Silver RAT v1.0 written in C Sharp is a Window based RAT builder for windows systems, which has different features like Bypass AV, stealing browser cookies, keylogger, hidden browser, hidden RDP access and much more.

pic

The builder section of Silver RAT, where users will find numerous options. Some notable features include the ability to Bypass AV, conceal malicious processes by assigning custom process names, and specify the connection method. The user can choose between default connection settings by providing an IP for reverse connection or opt for a web HTML link.

pic


Below is a list of the arguably most interesting functionalities of Silver RAT v1.0:

The attacker can utilize either an IP address with a specified port, or a webpage for command and control of the target system.
Windows defender exclusion function prevents detection after the program has been launched for the first time.
Attackers can configure this functionality to erase all system restore points. If the target attempts to turn off the system and run system restore, it will be ineffective.
This option can be configured to delay the execution of the payload. If the target runs the payload, it will not activate until the specified time has elapsed.
Hidden process and hidden installation, i.e. the capability to hide a process within the task manager. The attacker can provide a custom process name to hide the payload in a folder, which cannot be found even if the target tries to view hidden files or folders within Windows settings.
Bypassing Antivirus using FUD Crypters.

pic


ADMIN CONTROL PANEL
Upon successful connection, the attacker gains the ability to initiate various malicious activities on the target system, as seen in below snippet.

pic


Additionally, attackers can leverage other interesting malicious activities on target system such as:

Hidden Apps
– Attackers can control multiple applications on the client’s computer covertly, with various apps running concurrently.

Hidden Browsers
– Gives the ability to add client browsers to a hidden list.
– Enables the attacker and the victim to use the browser at the same time.

Hidden VNC
– Gives the attackers control of target system
– Attackers can control the client’s internet browsers.



