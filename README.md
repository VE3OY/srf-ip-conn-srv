# srf-ip-conn-srv
SharkRF IP Connector server automated installation for Raspberry Pi 3

After helping several HAM's perform the installation of SharkRF's IP Connector server,
it became obvious to me that the instructions out on the internet were either
incomplete or misleading.

I decided to write an automated installation for this great piece of software.

Assumption(s):

You own a Raspberry Pi 3, that has 1 GB of RAM and a 4 core ARM CPU.
You want to install and use this server software.
You are running, or are ok with running Raspbian Stretch.

What do you need to do to start?

Download the ZIP file that has everything you will need.

On your PC:
- create a temporary directory to work from (NOT c:\temp!)
- un-zip "IPC_Install.zip" into that directory

On your RPi:
- create a new sub-directory on your RPi:  mkdir /home/pi/IPC
- copy all of the un-zipped files from your PC, to that directory on your RPi
- at a command prompt, type the following commands:
	sudo su
	cd /home/pi/IPC
	chmod +x InstallIPConnectorV6.sh
	./InstallIPConnectorV5.sh

NOTES:
Pay close attention to upper/lowercase of the above commands!
It's CRITICAL!

Once the installation script runs, just follow any prompts.
Lots of information is shown, while the installation happens.

If you are running this installation on an existing Raspbian, then errors may happen.

No warranty or guarantee is made or implied.
Your mileage may vary!
Good luck, and enjoy!

Matt
ve3oy [at] ve3oy [dot] com
31DEC2018
