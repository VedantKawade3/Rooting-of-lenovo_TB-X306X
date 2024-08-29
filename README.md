# Rooting-of-lenovo_TB-X306X

<h1 align="center">Root lenovo tab M10 Hd (TB-X306X)</h1> <br><br>

<h4 style="color: red;">⚠️DISCLAIMER :- Do it at your own risk , I won't be responsible if anything goes wrong, you might risk to brick your tablet </h4> <br><br>

<p>•Step by step rooting process of lenovo TB-X306X :- <br> there are three steps to route Lenovo TB-X306X .</p>

1] Unlocking bootloader<br>
2] Patching recovery image using magisk app<br>
3] Flashing patched image in Lenovo TB-X306X using PC <br><br><br>

<h4>1] Unlocking bootloader :-</h4><br>
<h4>⚠️warning :- Unlocking bootloader wipes data on the device. It is recommended to backup your data. Proceed at your own risk .</h4><br><br>

I) To unlock bootloader open settings .<br><br>
II) Now click on system .<br>
        image1.png 
<br><br>
III) Click on about tablet .<br>
        image2.png
<br><br>
IV) Click 7 to 8 times on build number<br><br>
V) Now you are in developer mode and go back and open developer options. <br>
        image3.png 
<br><br>
VI) enable ```USB debugging``` and ```OEM unlocking``` & close settings.<br>
        image4.PNG<br>
        image5.PNG 
<br><br>
VII) Power off device and put it in ```fastboot mode``` by pressing ```power button``` + ```volume down button``` Simultaneously .<br><br>
VIII) Now download ```adb drivers``` in your pc and create platform-tools folder in C-drive and extract downloaded ADB drivers` zip (Platform-tools-latest-Windows.zip) file.
      You can download from <a href="https://dl.google.com/android/repository/platform-tools-latest-windows.zip" target="_blank">here</a> or from <a href="https://developer.android.com/tools/releases/platform-tools" target="_blank"> official website</a>. <br><br>

IX) Go to the folder where you extracted adb drivers` zip file and open cmd (command prompt or powershell) in that folder and connect to the tablet which we put in fastboot mode .<br><br>
X) Run following commands in cmd after tablet is connected to pc via usb cable .<br><br>
i) command 1 :<br>
```
fastboot devices
```
And hit enter , You will see your device name if it is not showing, then adb drivers are not properly installed, So reinstall it or update it .
if this doesn't work then check your usb cable is properly connected or not .
<br><br>
ii) command 2 :
```
fastboot flashing unlock
```
or 
```
fastboot oem unlock
```
or 
```
fastboot oem unlock-go
```
And hit enter Then on tablet screen, you will see it is asking you to press volume up to unlock or volume down to not unlock then press volume up to unlock bootloader .
<br><br><br>
<h4>2] Patching recovery image using magisk app :-</h4><br><br>

I) Install Lenovo software fix app in PC from  <a href="https://download.lenovo.com/consumer/mobiles/software_fix_v7.0.3.17_setup.exe" target="_blank">here</a> or you can download from <a href="https://pcsupport.lenovo.com/in/en/products/tablets/lenovo/lenovo-tablet-10/downloads/ds101291"> official website</a> .<br><br>
II) Connect your lenovo tab & open downloaded software fix app and in rescue option select your device type. After that, use usb connection section in it and download latest update for your device.<br>
                image10.png<br>
                image11.png
<br><br>
III) After download, it will show where your update is downloaded go there and find boot.img image and copy it and paste in tablet`s storage at known path (Any path you remember)
IV) Download magisk app in tablet from <a href="https://github.com/topjohnwu/Magisk/releases/download/v27.0/Magisk-v27.0.apk" target="_blank">here</a> or from <a href="https://magisk.me/apk/" target="_blank"> official website</a> . After that, open magisk app and click on install as shown<br>
                    image6.Png <br><br>
                    
V) click on ```select and patch a file``` option, and then click on ```LET`S GO``` option. After that, at the end. It will show directory where patched image is stored.<br>
                     image7.PNG<br><br>
VI) Go there and copy paste in your pc where adb drivers are installed .<br>
                     image9.png<br><br><br>

<h4>3] Flashing patched image in Lenovo TB-X306X using PC :-</h4> 
<br><br>
I) Open cmd in adb driver's directory .<br><br>
 
II) Type following command and hit enter ,<br>

i) command 1 : <br>
```
fastboot devices
```
If there is no device showing, then put your tablet in fastboot mode and connect it to PC via USB cable and then try this command again. If this doesn't work, check cable is properly connected or not .
<br><br>
ii) command 2 : 
```
fastboot flash boot magisk_patched-27000_rCLm6.img
```
image8.png
<br><br>
Now you successfully rooted your tablet , To check download root checker app from play store and check .

<img src="path/to/your/image.jpg" alt="Description of the image">
