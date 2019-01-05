# srf-ip-conn-srv
<H1>SharkRF IP Connector server AUTOMATED installation for Raspberry Pi 3</H1>

<H4>After helping several HAM's perform the installation of SharkRF's IP Connector server,
it became obvious to me that the instructions out on the internet were either
incomplete or misleading.
<br>
I decided to write an automated installation for this great piece of software.<br>
<br>
Assumption(s):
--------------
You own a Raspberry Pi 3, that has 1 GB of RAM and a 4 core ARM CPU.<br>
You want to install and use this server software.<br>
You are running, or are ok with running Raspbian Stretch.<br>
<br>
What do you need to do to start?<br>
<br>
Download the ZIP file that has everything you will need.<br>
<br>
On your PC:<br>
- create a temporary directory to work from (NOT c:\temp!)<br>
- un-zip "IPC_Install.zip" into that directory<br>
<br>
On your RPi:<br>
- create a new sub-directory on your RPi:  mkdir /home/pi/IPC<br>
- copy all of the un-zipped files from your PC, to that directory on your RPi<br>
- at a command prompt, type the following commands:<br>
	sudo su<br>
	cd /home/pi/IPC<br>
	chmod +x InstallIPConnectorV6.sh<br>
	./InstallIPConnectorV5.sh<br>
<br>
NOTES:
------
Pay close attention to upper/lowercase of the above commands!<br>
It's CRITICAL!<br>

Once the installation script runs, just follow any prompts.<br>
Lots of information is shown, while the installation happens.<br>
If you are running this installation on an existing Raspbian OS, then errors may happen.<br>
No warranty or guarantee is made or implied.<br>
Your mileage may vary!<br>
Good luck, and enjoy!<br>
<br>
Matt<br>
ve3oy [at] ve3oy [dot] com<br>
31DEC2018<br>
