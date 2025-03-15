# galaxy_gear_s3
Galaxy Deploy Solution


```
HOW TO INSTALL A WGT/TPK FILE ON YOUR WATCH?​
Keep in mind that this does not require root on your watch.

1. Open ‘Settings’ on your watch, go to ‘About watch’ --> ‘Debugging’ and turn ‘Debugging’ on. Do not forget to turn it off when you have finished installing the WGT file.
2. Turn on Wi-Fi on your watch and connect to a network. Once connected, click on your connected network to retrieve the IP address of your watch.
3. Download SDB on your Windows, Ubuntu or macOS device, and extract the SDB archive you need. Check release of repo. Make sure your device is connected to the same network as your watch.
4. Enter the extracted folder, go to ‘data/tools’ and open the command prompt here or navigate to ‘data/tools’ in the command prompt.
5. Type the following in the prompt on Windows: sdb devices. On Ubuntu and macOS, type the following in the prompt: ./sdb devices.
6. Type the following in the prompt on Windows: sdb connect [Gear S3 IP address]:26101. On Ubuntu and macOS,
    type the following in the prompt: ./sdb connect [Gear S3 IP address]:26101.
    If SDB cannot find your wearable, open ‘Settings’ on your watch, go to ‘About watch’ --> ‘Debugging’, and toggle ‘Debugging’ off and on.
    Then reboot your watch and repeat this step. Also, make sure you keep the watch screen on!
    Now, there will be an RSA key request on your watch. Accept it.

Type the following in the prompt on Windows: s
  db install [Path to the WGT file]/[Name of the WGT file].wgt.

  On Ubuntu and macOS, type the following in the prompt: ./sdb install [Path to the WGT file]/[Name of the WGT file].wgt.

  Once the installation is complete you might get a message like ‘rm: remove write-protected regular file ‘/opt/usr/home/owner/apps_rw/tmp/[Name of the WGT file].wgt’?’.
  On Windows and Ubuntu, use CTRL + C to proceed. On macOS, use Command + . to proceed. For a TPK file,
  just change the ‘.wgt’ in the commands to ‘.tpk’.

  When you are done, please do not forget to kill the SDB server. Type the following in the prompt on Windows: sdb kill-server. On Ubuntu and macOS, type the following in the prompt: ./sdb kill-server.
  That is all. I hope this has been helpful to you all. If you need any help of have any questions, please reply on the thread.
```


Running instructions for my device
```
sdb connect 192.168.0.46:26101

sdb install "C:\development\gear\Tinzen Nolische Gear Workspace\GearWatchDesigner\workspace\NolischeWatchFace.tpk"

sdb push "C:\development\gear\Tinzen Nolische Gear Workspace\GearWatchDesigner\workspace\NolischeWatchFace.tpk" /tmp/nolische_watch_face.tpk
```
