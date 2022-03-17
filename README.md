# Tesseract-Cobra
### This Project is a Collection of Tools, Firmware and Information and wasent authorized by LYRobotix/NOLO Co., Ltd.
### Warning, i am not responsible if you do Brick your Device and make it unusable.
### Please read all Instructions carefully.

Goal of this Project is to help Users of Nolo Hardware to flash their Hardware manually and without the usage of the Updaters.
Its also our Target to make this Process as simple as possible, and to avoid bricking Hardware.
#

|-Warnings
- Do not manually flash your Device if you feel insecure about it or may not have the required Knowledge
- Be absolutly sure you do use the correct Firmware, only use Files from "/Firmware/Official/"
- Do not have multiply Nolo Devices connected at the same Time
- Use an proper USB Cable, having an loose Connection could interrupt the flashing Procedere and damage your Device
- If you have any further Questions, create an Issue or ask support@nolovr.com

#
|-Flashing Manually
1. Lookup "Hardware Identifiers.txt" to find out your Hardware Model  
2. Go to "/Drivers" and Install the ST32 Driver for CV1 Pre-Sale Devices or the GD32 Driver for regular CV1 Devices (idk about Nolo Home yet, propably its GD32)  
3. Bring your Device into DFU Mode, Information on how todo can be found in "Enter Recovery and DFU-Mode.md"
4. Go to "/Tools" and go to "DfuSe" for flashing CV1 Pre-Sale Devices and "GD32" for regular CV1 Devices (idk about Nolo Home yet, propably its GD32)  
5. A: For ST32, open up "/Bin/DfuSeDemo.exe"  
   B: For GD32, Open up "GD32 MCU Dfu Tool.exe"  
6. A: For ST32, select the Device in the upper Drop-Down Menu. If you see more then one Device, unplug your Hardware to find out which Device to use. Some Bluetooth Adapters are always in DFU mode, you may temporary disable them in the Device Manager.  
   B: For GD32, click "No" when the Software asks for an Update. Select the Device in the upper Drop-Down Menu. If you see more then one Device, unplug your Hardware to find out which Device to use. Some Bluetooth Adapters are always in DFU mode, you may temporary disable them in the Device Manager
7. Download the required Firmware coresponding to your Device from "/Firmware/Official"  
8. A: For ST32, click on "Choose..." in the "Upgrade or Verify Action" Section [>Picture<](https://i.imgur.com/EGJGmwb.png). Navigate to the previously downloaded Firmware and select it. Click "Upgrade" to start the flashing Procedure, do not disconnect the Device now!  
   B: For GD32, change the starting Adress in the "Download APP program file" Section, from 8000000 to 8003000 [>Picture<](https://i.imgur.com/134D1aR.png). click on "open" [>Picture<](https://i.imgur.com/1ANDMG1.png). In the Lower right, select "BIN Files" [>Picture<](https://i.imgur.com/dLXJNxa.png). Navigate to the previously downloaded Firmware and select it. Click "OK" in the lower right to start the flashing Procedure, do not disconnect the Device now!  
