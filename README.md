<h1 align="center">Analyzing disk image of suspect's computer to extract data that would be useful in an investigation</h1>

In this lab from SBT’s Blue Team Level 1 course we’ll be analyzing a disk image of a suspect’s laptop to find important information that could be useful in an investigation.

<h3 align="center">What operating system and OS version is the suspect laptop running?</h3>
On the left hand panel we can see various categories that store different types of data and information about the laptop and we need to see which category would have the relevant data that the question is asking.
Data Artifacts > Operating System Information:

<h3 align="center">What is the hostname of this system?</h3>
Also within Operating System Information:

<h3 align="center">What is the name of the file that was downloaded at 2013-12-18 20:05:57?</h3>
We need to figure out where data about downloads would be stored in Autopsy.
Data Artifacts > Web Downloads:

<h3 align="center">Where can you find the FQDN of the file that was downloaded 2013-12-18 03:02:50?</h3>

<h3 align="center">What is the actual file path for the Pier lnk file?</h3>
.lnk files are basically shortcut files, it isn’t the actual file, it just contains information about where that specific file is located. An example would be creating a desktop shortcut of any file or folder that is stored somewhere else so that desktop icon you see is actually a .lnk file. Based on this and from the categories presented in Autopsy let’s try searching in Data Artifacts > Recent Documents: 

<h3 align="center">When was the local administrator account last accessed?</h3>
OS Accounts:


<h3 align="center">What is the size of the laptop image?</h3>
Data Sources > Craig Tucker Desktop.E01_1 Host:

For a better understanding of how big this laptop image is, convert bytes to GB to get 64.424GB.
