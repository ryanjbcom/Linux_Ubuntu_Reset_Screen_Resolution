Linux_Ubuntu_Reset_Screen_Resolution
====================================

Linux, Ubuntu 14.04 (maybe all versions), script &amp; instructions to reset the screen resolution. 

Ryan Bridglal
June 11th, 2014

This is a script I just created to reset the screen resolution.

I accidentially set a resolution too high, in which my monitor could not detect (1650x1080).

When the pc rebooted, I was unable to see the video. All I got was a message on my screen saying the screen mode can't be displayed, please set a resolution of 1440x900.


At this point, on my keyboard I hit (at the same time):

CTRL + ALT + F1



This brought me to a new terminal login screen. I Entered my user name and password and I had a good working command prompt.


The next step was to manually rewrite a configuration file for the xorg display system of my machine.

I entered:

sudo nano /etc/X11/xorg.conf


This worked out great and opened the file; mine was blank (scary).

At this point I typed out the code you can review in the code file and saved it. Then I entered:

sudo reboot

EVERYTHING WAS BACK TO NORMAL!
