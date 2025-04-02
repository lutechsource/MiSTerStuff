[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/Dw0jmcvMoNQ/0.jpg)](https://www.youtube.com/watch?v=Dw0jmcvMoNQ)

## **Pre-requisites**

* Retro Shooter light guns
  * Available at https://retroshooter.com/
* Make sure your MiSTer FPGA is up-to-date, so run update_all
* At the moment, an unstable Linux kernel is required. 
  * Download the kernel here (Choose the Jan 13 2025): [https://github.com/MiSTer-unstable-nightlies/Linux-Kernel\_MiSTer/releases](https://github.com/MiSTer-unstable-nightlies/Linux-Kernel_MiSTer/releases)
  * Rename the downloaded file to zImage_dtb
  * Copy it to the **/media/fat/linux/** directory on your SD Card. Make sure to backup the current zImage_dtb, in case something goes wrong.
* A keyboard (So you can press F10 to bring up the calibration menu)

### 1.  **Calibrate Lightguns on PC**

This step might not be required but if you are experiencing calibration issues then perform this. Connect your Light guns to a Windows PC and run it’s calibration software. The software is obtained from Retro Shooter’s private facebook group.

Retro Shooter Facebook group:

[https://www.facebook.com/groups/278774617977291](https://www.facebook.com/groups/278774617977291)

### 2. **Connect Light guns to MiSTer FPGA**

* Connect the Retro Shooter Base station to your MiSTer FPGA and the light guns to the base station.
* Power your MiSTer and go to Define Joystick Buttons in the main menu screen (With no core loaded).
* Define the buttons on the light gun the way you like. To skip a key mapping press the USER button on your MiSTer FPGA.
  * Since the light gun is seen as a keyboard you will not be able to use space to skip a key mapping. Even if you have another keyboard plugged in you will not be able to use its space button. Instead you will have to use your MiSTerFPGA’s physical USER button.
* After you’re done configuring buttons you can start loading cores, but they also need to be configured.



**Below are some core specific guides, I’m still testing the lightgun so I’ll add more cores as I do more testing.**

## **Atari 7800 Core**

> [!WARNING]  
> I couldn't get this core to calibrate at all. However, if you may be more successful, so below are the instructions for the Atari 7800.


* Bring up core menu.
* Go to **Define Atari 7800 buttons.** Below are what buttons pertain to what light gun controls.
  * 7800 Fire1: Lightgun trigger
* Now Go to **Peripherals** option in the main core menu and use these settings
  * **Port1 or 2 Input:** Lightgun. You can also see if "Auto" works. 
    * Choosing port 1 or 2 depends what player you light gun was set to when you loaded the core
  * **Gun X Tunning:** (I have no idea what it does)
  * **Gun Control:** Joy1 or Joy2.
    * Depends what player you light gun was set to when you loaded the core
  * **Gun Fire:** Joy
  * **Cross:** Your crosshair preference.
* Load a lightgun game
  * Calibrate the gun for the core. Bring up the core menu and press **F10** on your keyboard. Follow the calibration instructions. 
    * Calibrate to the viewable 4:3 area of the core screen. NOT the entire size of a 16:9 screen. A game screen that has no black will make this easier.
  * You might need to change the **Gun Control** setting if the lightgun isn’t working. If it’s at **Joy1** then change it to **Joy2** or vice versa.
  * You may also need to calibrate using a games built-in calibration tool
  * If you experience further calibration issues, you may need to calibrate your light gun in Windows.
* Enjoy your game!


## **Genesis Core (Not the MegaDrive core)**

I haven’t tested the Mega Drive core yet.

* Bring up core menu.
* Go to **Define Genesis buttons**
  * Define the buttons on the light gun the way you want. However, make sure that when you get to **Button A**, you map it to the **trigger** of the light gun.
* Now Go to **Input** option in the main core menu and use these settings
  * **Gun Control:** Joy1 or Joy2. 
    * It all depends what player you light gun was set to when you loaded the core
  * **Gun Fire:** Joy
  * **Crosshair:** Your preference.
* Load a lightgun game
  * Calibrate the gun for the core. Bring up the core menu and press **F10** on your keyboard. Follow the calibration instructions. 
    * Calibrate to the viewable 4:3 area of the core screen. NOT the entire size of a 16:9 screen. A game screen that has no black will make this easier.
  * You might need to change the **Gun Control** setting if the lightgun isn’t working. If it’s at **Joy1** then change it to **Joy2** or vice versa.
  * You may also need to calibrate using a games built-in calibration tool
  * If you experience further calibration issues, you may need to calibrate your light gun in Windows.
* Enjoy your game!

## **NES Core**

* Bring up core menu.
* Go to **Define NES buttons**
  * Define the buttons on the light gun the way you want. However, make sure that when you get to **Zapper/Vaus Btn**, you map it to the **trigger** of the light gun.
* Go to **Input Options** and use these settings
  * **Periphery: Zapper (Joy1) or Zapper(Joy2).** 
    * It all depends what player you light gun was set to when you loaded the core
  * **Zapper Trigger:** Joystick
  * **Crosshair:** Your preference.
  * **Swap Joysticks:** Change this in some cases if the lightgun is not working. This will change the player 1 controller to player 2 and vice versa.
* Load a lightgun game
  * Calibrate the gun for the core. Bring up the core menu and press **F10** on your keyboard. Follow the calibration instructions. 
    * Calibrate to the viewable 4:3 area of the core screen. NOT the entire size of a 16:9 screen. A game screen that has no black will make this easier.
  * Remember you might need to change the **Swap Joysticks** settings if the lightgun isn’t working.
  * You may also need to calibrate using a games built-in calibration tool
  * If you experience further calibration issues, you may need to calibrate your light gun in Windows.
* Enjoy your game!

## **PSX Core**

* Bring up core menu.
* Go to **Define PSX buttons**. Below are what buttons pertain to what light gun controls.
  * Start:GunCon A (If you are going to use the Retro Shooter Pedals then you will want to map this to the pedal, because it’s what controls ducking in Time Crisis).
  * O: Trigger
  * X: Guncon B
* Now go to the main core menu page use these settings
  * **Pad 1 or Pad2:** Guncon or Justifier
    * Pad depends what player your light gun was set to when you loaded the core. Guncon or Justifier depends on what game you are playing.
  * **Show Crosshair:** Your preference.
* Make sure to save your settings if you do not want to make these changes the next time you load the core.
* Load a lightgun game
  * Calibrate the gun for the core. Bring up the core menu and press **F10** on your keyboard. Follow the calibration instructions. 
    * Calibrate to the viewable 4:3 area of the core screen. NOT the entire size of a 16:9 screen. A game screen that has no black will make this easier.
  * You may also need to calibrate using a games built-in calibration tool
  * If you experience further calibration issues, you may need to calibrate your light gun in Windows.
* Enjoy your game!

## **Saturn Core**

* At the moment an unstable Saturn core build is necessary.
  * Download latest rbf from here: https://github.com/MiSTer-unstable-nightlies/Saturn_MiSTer/releases/tag/unstable-builds  
* Bring up core menu.
* Go to **Define Saturn buttons**. Below are what buttons pertain to what light gun controls. Just map the two buttons below
  * Saturn A button: Gun Trigger
  * Saturn Start button: Gun Start
* Now go to the main core menu page use these settings
  * Go to **Input**
  * **Pad 1 or Pad2:** Virt LGun
    * Pad depends what player your light gun was set to when you loaded the core. Guncon or Justifier depends on what game you are playing.
    * **LGun PX XY Ctrl:** Joy X
    * **LGun PX Buttons:** Joy X
    * **LGun P2 Crosshair:** Your preference
* Make sure to save your settings if you do not want to make these changes the next time you load the core.
* Load a lightgun game
  * Calibrate the gun for the core. Bring up the core menu and press **F10** on your keyboard. Follow the calibration instructions.
    * Calibrate to the viewable 4:3 area of the core screen. NOT the entire size of a 16:9 screen. A game screen that has no black will make this easier.
  * You may also need to calibrate using a games built-in calibration tool
  * If you experience further calibration issues, you may need to calibrate your light gun in Windows.
* Enjoy your game!

## **SNES Core**

* Bring up core menu.
* Go to **Define SNES buttons**
  * Define the buttons on the light gun the way you want.
  * SNES A (SS Fire) : Lightgun trigger
  * SNES B (SS Cursor): your choice of button on the lightgun
  * SNES X (SS TurboSW): your choice of button on the lightgun
  * SNES Y (SS pause): your choice of button on the lightgun
  * LT(SS Cursor): your choice of button on the lightgun. Not required if you already mapped A
  * RT(SS Fire): your choice of button on the lightgun. Not required if you already mapped B
* Go to **Input Options** and use these settings
  * **Super Scope:** Joy1 or Joy 2
    * It all depends what player you light gun was set to when you loaded the core
  * **Super Scope button:** Joys
  * **Crosshair:** Your preference.
  * **Gun Type:** Depends on the game. Konami games use justifier. All other games should be super scope (not 100% on this so try switching this if a game does work)
  * **Swap Joysticks:** Change this in some cases if the   is not working. This will change the player 1 controller to player 2 and vice versa.
--------------------


* Load a lightgun game
  * Calibrate the gun for the core. Bring up the core menu and press **F10** on your keyboard. Follow the calibration instructions. 
    * Calibrate to the viewable 4:3 area of the core screen. NOT the entire size of a 16:9 screen. A game screen that has no black will make this easier.
  * Remember you might need to change the **Swap Joysticks** settings if the lightgun isn’t working.
  * You may also need to calibrate using a games built-in calibration tool
  * If you experience further calibration issues, you may need to calibrate your light gun in Windows.
* Enjoy your game!

