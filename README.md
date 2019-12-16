# Tesseract-Cobra
### Warning, i am not responsible if you do Brick your Device and make it unusable.
### Please read all Instructions carefully.

Goal of this Project is to help Users of Nolo Hardware to flash their Hardware manually and without the usage of the Updaters.
Its also our Target to make this Process as simple as possible, and to avoid bricking Hardware.
#
|-Problems  
 |Device wont turn on - Probably, the wrong Firmware is flashed  
 |Device LED wont turn on - Try to hold down the Power Button, plug in the Device to a USB Power Outlet or do go into Recovery Mode  
 |Device LED stays dark even when holding the Power Button or Charging - The Main Firmware is damaged, enter Recovery Mode and flash manually
 |Device wont turn into Recovery Mode - The wrong Firmware is flashed  
 |The Device turns on and off - Either the Driver is installed inproperly or the Battery is empty, try to reinstall the Driver and charge your Controller or Base Station  
 |The Device turns on and off once in Recovery mode - Either the Driver is installed inproperly or the Firmware on the Device is damaged. If reinstalling the Driver does not help, hold down the Recovery Mode Keys and flash the Firmware manually before it restarts again  
 |Device wont pair - Maybe the Firmware across the Devices is different, bring all of them to a similar Version  
#
|-Flashing Manually
1. Lookup "Hardware Identifiers.txt" to find out your Hardware Model  
2. Go to "/Drivers" and Install the ST32 Driver for CV1 Pre-Sale Devices or the GD32 Driver for regular CV1 Devices (idk about Nolo Home yet, propably its GD32)  
3. A: Bring your Device into DFU Mode by pressing the right Buttons at the right Time as shown in the Nolo Updater, the LED should be flashing Orange  
3. B: If you do not have Succes with Methode A, do try to bring your Device into DFU Mode by using the Nolo Firmware Updater  
4. Go to "/Tools" and go to "DfuSe" for flashing CV1 Pre-Sale Devices and "GD32" for regular CV1 Devices (idk about Nolo Home yet, propably its GD32)  
5. A: For DfuSe, open up "/Bin/DfuSeDemo.exe"  
   B: For GD32, Open up "GD32 MCU Dfu Tool.exe"  
6. A: For DfuSe, select the Device in the upper Drop-Down Menu. If you see more then one Device, unplug your Hardware to find out which Device to use.  
   B: For GD32, click "No" when the Software asks for an Update. Select the Device in the upper Drop-Down Menu. If you see more then one Device, unplug your Hardware to find out which Device to use.  
7. Download the required Firmware coresponding to your Device from "/Firmware/Official"  
8. A: For DfuSe, click on "Choose..." in the "Upgrade or Verify Action" Section(https://i.imgur.com/EGJGmwb.png). Navigate to the previously downloaded Firmware and select it. Click "Upgrade" to start the flashing Procedure, do not disconnect the Device now!  
   B: For GD32, click on "open" in the "Download APP program file" Section(https://i.imgur.com/1ANDMG1.png). In the Lower right, select "BIN Files"(https://i.imgur.com/dLXJNxa.png). Navigate to the previously downloaded Firmware and select it. Click "OK" in the lower right to start the flashing Procedure, do not disconnect the Device now!  

#
|-Device LED Status Codes  
![Device LED Status Codes](https://i.imgur.com/YZ58YsV.png)
