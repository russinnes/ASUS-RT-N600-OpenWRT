# ASUS-RT-N600-OpenWRT
OpenWRT Build (22) for the ASUS N600 router

This binary firmware is for the Asus RT-N600 Router and contains OpenWrt SNAPSHOT r19805-574539ee2c / LuCI Master git-22.167.28356-8effea5

This must be initially flashed using the ASUS recovery tool, or as an upgrade from a previously flashed aftermarket firmware. 
Flashing from Padavan (If you are running my previous build) will not work. 
A google search of Asus firmware restoration, using their tool will point you to it. 
Essentially, set a static IP in the 192.168.1.10+ range, power on the device while holding 
reset (LED will flash), then run the restore tool, selecting the image you want to flash (in this case, 
the OpenWRT .squashfs sysupgrade image for most folks).

Everything is working except for the 5g WiFi LED. I'll keep plugging away at it. 

** NOTE **
There is also the image for the AC1200 here, which works on the RT-N600 including the 5g LED
However - It's a snapshot without Luci; so;
-SSH into the box (root@192.168.1.1);opkg update;opkg install luci;


I plan to commit this board and the associated configs to the OpenWRT master when I get some more time. 

This puts a ton of power behind this router that is a few years old now. 

