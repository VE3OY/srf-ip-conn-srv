# srf-ip-conn-srv
<H1>SharkRF IP Connector server AUTOMATED<br>installation for Raspberry Pi 3</H1>

<H4>After helping several HAM's perform the installation of SharkRF's IP Connector server,<br>
it became obvious to me that the instructions out on the internet were inaccurate.
<br>
I decided to write an automated installation for this great piece of software.<br>
<br>
Assumption(s):<br>
----------------<br>
You own a Raspberry Pi 3, that has 1 GB of RAM and a quad core ARM CPU.<br>
You want to install and use this server software.<br>
You are running, or are ok with running Raspbian Stretch.<br>
You have a working internet connection for your Raspberry Pi.<br>
<br>
Here is what you need to start:<br>
-----------------------------------<br>
Begin by putting a fresh image of Raspbian Stretch onto your Raspberry Pi.<br>
Set up your Pi (hostname/timezone/etc).<br>
<br>
Download the ZIP file that has everything you will need.<br>
<br>
On your PC:<br>
- create a temporary directory to work from (NOT c:\temp!)<br>
- un-zip the downloaded file into that directory<br>
<br>
On your Raspberry Pi:<br>
- create a new sub-directory:<br>
<ol>mkdir /home/pi/IPC</ol>
- copy all of the un-zipped files from your PC to that new directory<br>
- at a command prompt, type the following commands:<br>
<ol>sudo su<br>
cd /home/pi/IPC<br>
chmod +x InstallIPConnectorV6.sh<br>
./InstallIPConnectorV6.sh</ol>
<br>
NOTES:
  -----<br>
Pay close attention to upper/lowercase of the above commands!<br>
It's CRITICAL!<br>
<br>
This installation routine will do the following:<br>
- Update and upgrade your Raspbian OS<br>
- Install NGINX (rather than APACHE2) and PHP<br>
- Install NTP (Network Time Protocol)<br>
- Disable the default 100MB swap file<br>
- Install ZRAM swap in RAM (not file!)<br>
- Install the IP Connector as a service, so it auto-restarts after a failure or reboot.<br>
<br>
Once the installation script runs, just follow any prompts.<br>
Lots of information is shown, while the installation happens.<br>
If you are attempting to install this on another Raspbian OS, then errors may happen.<br>

Important:
-----------
For this program to work, you need to set up port-forwarding on your router/firewall<br>
so that Port 65100 is open to the internet.  If this port is not opened, then nobody<br>
outside of your home network will be able to connect to it.

No warranty or guarantee is made or implied.<br>
Your mileage may vary!<br>
Good luck, and enjoy!<br>
<br>
Matt<br>
ve3oy [at] ve3oy [dot] com<br>
31DEC2018<br>
</H4>
