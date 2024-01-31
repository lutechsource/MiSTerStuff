Groovy MiSTer project Github: https://github.com/psakhis/Groovy_MiSTer

#Instructions

###Requirements
-These instructions use MAME on a Windows computer.

-Make sure the MiSTerFPGA is setup for analog video output. Refer to the CRT section of the MiSTerFPGA documentation. (https://mister-devel.github.io/MkDocs_MiSTer/advanced/crttable/)

**Required files, available for download at: https://github.com/psakhis/Groovy_MiSTer/tree/main/test-builds)**
Groovy.rbf
MiSTer (Replaces the MiSTer file on your MiSTerFPGA installation)
mame_nogpu_24.7z

Also, ethernet is required for the best performance. Avoid using Wifi. 
You can also use an ethernet cable to connect the MiSTerFPGA to a PC directly.



On the MiSTerFPGA:
Copy Groovy.rbf to the file to the /media/fat/_Utility folder.
Rename the MiSTer file in /media/fat to MiSTer.bak.
Copy the newly downloaded MiSTer file from the Groovy github to /media/fat.

It’s best to have a static IP address set for you MiSTerFPGA. You do that by:
Editing the  /etc/dhcpcd.conf file on the MiSTer FPGA SDCard.
Add these two lines at the end, replacing the your_static_ip_here with the ip address you want to use on the MiSTer

interface eth0
static ip_address=your_static_ip_here/24


On the PC:
Extract mame_nogpu_24.7z to a current MAME installation. This will replace the mame.exe file, so rename the current one if you want to or just create a copy of the MAME installation just for GroovyMiSTer.

Create a Windows shortcut or batch file in the MAME installation directory that runs this command:
mame -video mister -aspect 4:3 -switchres -monitor arcade_15 -mister_window -mister_ip "192.x.x.x" -mister_compression lz4 

Replace 192.x.x.x with the IP address. Leave the quotes on the ip address.

On PC & MiSTer:
Connect MiSTerFPGA and PC to the same ethernet network. The faster the better.

Or, if you can, connect the PC and MiSTer directly to each other using one ethernet cable.
You can still use Wifi to connect the internet on both the PC and MiSTer if you have wifi adapters installed..

On the MiSTer:

Load up the GroovyMiSTer core in the Utilities folder when you boot up.
A scrolling blue circle with red,blue,green slashes will move around the screen.
The MiSTer is now ready to accept a connection to the PC.

On the PC:
Run the mame batch file or shortcut that runs the command where you set the IP address.
Mame will now boot up on both the MiSTer and PC.

Controls are handled through the PC. You CANNOT use controllers connected to MiSTer to play games over Groovy MiSTer.

Remember you will have to configure MAME with controls and location of your games.
