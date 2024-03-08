This is a guide to setting up MiSTerCast. I have an overview video of MiSTerCast here: https://youtu.be/vCjbmVQwM6Q

# Requirements
- Groovy MiSTer setup on MiSTerFPGA. It is in Section 1 from [here](https://github.com/lutechsource/MiSTerStuff/blob/main/GroovyMiSTer/mame_documentation.md#section-1-on-the-misterfpga)
- MiSTerCast software by Shane Lynch available  [here](https://github.com/iequalshane/MiSTerCast/releases). There is also a link there to the Microsoft VC++ x86 Redistributable. Make sure to install that also if it's already not installed on your computer.

# Instructions

1. Complete Section 1 from my Groovy MiSTer MAME setup guide found [here](https://github.com/lutechsource/MiSTerStuff/blob/main/GroovyMiSTer/mame_documentation.md#section-1-on-the-misterfpga)

2. Make sure the  MiSTer FPGA are connected to the same network, or straight to each other using an ethernet cable. Wifi is very unstable so do not use it.

3. Run the Groovy MiSTer core on the MiSTer FPGA. Doing this will prepate the MiSTer to recieve a connection from the PC.
    1. If you want sound output from the MiSTerFPGA, on the MiSTer FGPA, bring up there core menu select "Audio Setttings" then set "Audio" to "On."
![Enable Audio Groovy MiSTer](https://github.com/lutechsource/MiSTerStuff/blob/main/GroovyMiSTer/groovy_mister_enable_audio.gif)

4. Download the MiSTerCast application (Link above in requirements). Extract zip and run MiSTerCast.exe
    1. If you want sound to be output from the MiSTerFPGA check off "Enable Sound"
![Enable Audio MiSTerCast](https://github.com/lutechsource/MiSTerStuff/blob/main/GroovyMiSTer/mistercast_enable_audio.png)
    2. If you have multiple monitors select the monitor you want to output to by selecting it in the Display dropdown located in the "Capture Source" section.
![Select monitor](https://github.com/lutechsource/MiSTerStuff/blob/main/GroovyMiSTer/mistercast_monitors.png)

5. On the "Target IP" textbox enter the IP address of the MiSTerFPGA's ethernet port and then click "Start Stream"
![Inser IP address](https://github.com/lutechsource/MiSTerStuff/blob/main/GroovyMiSTer/mistercast_targetIP.png)

6. Your desktop will now appear on the CRT. Look below for an overview of the options to customize your experience.

# MiSTerCast Options
>[!CAUTION]
This section is still being worked on.
