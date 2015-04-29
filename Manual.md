# Introduction #
This script is designed to gather information on a possibly infected machine, including an NMAP scan, local users, local groups, NETSTAT, tasklist, and more.

# Requirements #
First, download the ZIP and extract it to a new folder.  In order to avoid any copywrite issues, I have not included any of the 3rd party programs.  Before using the `_run.bat` script, you will need to download and install some free tools.  These tools are:

  * PStools - http://technet.microsoft.com/en-us/sysinternals/bb896649.aspx
  * Autoruns - http://technet.microsoft.com/en-us/sysinternals/bb963902.aspx
  * NMAP - http://nmap.org/
  * Netscan - http://www.softperfect.com/products/networkscanner/

For each application, download the ZIP file version of the application and unzip it into the appropriate folder.  So the contents of the PSTools ZIP file go in the "pstools" folder, the contents of the NMAP ZIP file go in the "nmap" folder, etc.

# Usage #
After all 3rd party applications have been placed in their correct folders, you execute the `_run.bat` file with 2 arguments: the name of the target machine and the IP address of the target machine.

**Example**

`_run.bat machineName 10.11.12.13`

A new folder will be created under the "scans" folder named "machineName-YYYYMMDD".  All output from scripts and commands are placed in that folder.