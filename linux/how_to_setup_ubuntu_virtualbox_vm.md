**This document helps you to install and setup virtual box and load ubuntu desktop operating system into virtual box.**

Download links:  
Virtual Box : https://www.virtualbox.org/wiki/Downloads  
Ubuntu Desktop : https://ubuntu.com/download#download  

**Step 1**: Install Virtual Box with default options and click yes for any promts.  
**Step 2**:  Run the virtual box , Load and install ubuntu in virtual box.

Select the ubuntu image Left side and click on settings .   

Go to storage and select Ubuntu image from optical disk drive.    
Go to network and Adapter 1 Mapped to NAT and Adapter 2 Mapped to Host Only adapter.    
Go to Shared Folders and add Shared Folder.  

Start the VM and Follow the installation steps, and restart after complete.

**Full Screen Mode issue:**
Up on clicking full screen mode Rt_Ctrl+F , virtual box will not show ubuntu in full screen.  
You have not installed the Guest Additions (GAs). No GAs => no FullScreen.   
With the VM window having the focus, go to the host's menu "Devices" » "Insert Guest Additions CD Image...".   
If not prompted by auto-run, run "VBoxWindowsAdditions.exe" from the CD. Make sure there are no errors or suggestions during the install.  


**Enable SSH to connect from Putty**
Make sure ssh client is installed on your Linux. If not, install it **sudo apt install ssh**.  
Power off the OS.  
Now on your VB go to Settings -> Network -> on Adapter 2 choose Host-only adapter->click OK.  
Now start your OS. Run ifconfig; now the inet address is your IP.  
Use this and run it on your putty. Login with your credentials.  

**Install GIT**
sudo apt install git  
git --version  


**Install java 8**  
sudo apt install openjdk-8-jdk openjdk-8-jre

java --version

nano /etc/environment  
JAVA_HOME= /usr/lib/jvm/java-8-openjdk-amd64  
JRE_HOME=/usr/lib/jvm/java-8-openjdk-amd64/jre  








