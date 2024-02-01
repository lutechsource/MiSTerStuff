Groovy MiSTer project Github: [https://github.com/psakhis/Groovy_MiSTer](https://github.com/psakhis/Groovy_MiSTer)

### Requirements
- These instructions use MAME on a Windows computer.
- Make sure the MiSTerFPGA is setup for analog video output. Refer to the CRT section of the MiSTerFPGA documentation. (https://mister-devel.github.io/MkDocs_MiSTer/advanced/crttable/)
- **Required files, available for download at: https://github.com/psakhis/Groovy_MiSTer/tree/main/test-builds)**
  - **Groovy.rbf**
  - **MiSTer** file (Replaces the **MiSTer** file on your MiSTerFPGA installation)
  - **mame_nogpu_24.7z**
- Also, ethernet is required for the best performance. Avoid using Wifi.
  - You can also use an ethernet cable to connect the MiSTerFPGA to a PC directly.


# Instructions

### On the MiSTerFPGA:

- [ ] Copy Groovy.rbf file to the /media/fat/_Utility on MiSTer SD Card.
- [ ] Rename the **MiSTer** file in /media/fat to **MiSTer.bak**.
- [ ] Copy the newly downloaded **MiSTer** file from the Groovy github to /media/fat.
- [ ] Configure a static IP adress for the MiSTer.

**How to configure a Static IP on the MiSTer FPGA**

Edit the  /etc/dhcpcd.conf file on the MiSTer FPGA SDCard.
Add these two lines at the end, replacing the <your_static_ip_here> with the ip address you want to use on the MiSTer. This will set a static IP for the ethernet port, not Wifi.

```
interface eth0
static ip_address=<your_static_ip_here>/24
```

- [ ] Load up the GroovyMiSTer core in the Utilities folder when you boot up.
- [ ] A scrolling blue circle with red,blue,green lines will move around the screen. This means the MiSTer Groovy core is now ready to accept a connection from the PC.

![Loading Groovy core](https://github.com/lutechsource/MiSTerStuff/blob/main/GroovyMiSTer/booting_groovy_core.gif)

### On the PC:
- [ ] Extract **mame_nogpu_24.7z** to a current official MAME installation. This will replace the current mame.exe file, so rename the current one if you want to or just create a copy of the MAME installation just for GroovyMiSTer.
- [ ] Create a Windows shortcut or batch file in the MAME installation directory that runs the below command. Replace 192.x.x.x with the static MiSTer IP address. Leave the quotes on the ip address.

``
mame -video mister -aspect 4:3 -switchres -monitor arcade_15 -mister_window -mister_ip "192.x.x.x" -mister_compression lz4
``

### On PC & MiSTer:
- [ ] Connect MiSTerFPGA and PC to the same ethernet network. The faster the better.
  - Or, if you can, connect the PC and MiSTer directly to each other using one ethernet cable. You can still use Wifi to connect the internet on both the PC and MiSTer if you have wifi adapters installed.

### On the PC:
- [ ] Run the mame batch file or shortcut you created for running mame.
![Loading MAME on CRT](https://github.com/lutechsource/MiSTerStuff/blob/main/GroovyMiSTer/groovy_mister_gameloading.gif)

Mame will now boot up on both the MiSTer and PC.

>[!NOTE]
Controls are handled through the PC. You **CANNOT** use controllers connected to MiSTer to play games over Groovy MiSTer.
Remember you will have to configure MAME to fit your needs. Things like controls, location of your games, etc.
