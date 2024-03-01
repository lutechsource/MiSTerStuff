This is a guide to setting up MiSTerCast
>[!CAUTION]
WARNING! These instructions are NOT incomplete and still being worked on.

# Requirements
- Groovy MiSTer setup on MiSTerFPGA. Section 1 from [here](https://github.com/lutechsource/MiSTerStuff/blob/main/GroovyMiSTer/mame_documentation.md#section-1-on-the-misterfpga)
- MiSTerCast software by Shane Lynch available  [here](https://github.com/iequalshane/MiSTerCast/releases). There is also a link there to the Microsoft VC++ x86 Redistributable. Make sure to install that also if it's already not installed on your computer.

# Instructions

1. Complete Section 1 from my Groovy MiSTer MAME setup guide found [here](https://github.com/lutechsource/MiSTerStuff/blob/main/GroovyMiSTer/mame_documentation.md#section-1-on-the-misterfpga)

2. Make sure the  MiSTer FPGA are connected to the same network, or straight to each other using an ethernet cable. Wifi is very unstable so do not use it.

3. Run the Groovy MiSTer core on the MiSTer FPGA. Doing this will prepate the MiSTer to recieve a connection from the PC.

4. If you want sound output from the MiSTerFPGA, bring up there core menu select ?????? then ??????.

5. Download MiSTerCast application. Extract zip and run MiSTerCast.exe
    1. If you want sound to be output from the MiSTerFPGA check off "Enable Sound"
    2. If you have multiple monitors select the monitor you want to out by ????????????

6. On the "Target IP" textbox enter the IP address of the MiSTerFPGA's ethernet port and then click "Stream"

7. Your desktop will now appear on the CRT. Look below for an overview of the options to customize your experience.

# MiSTerCast Options

