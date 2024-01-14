# ntpq
Hobbit/Xymon NTPQ with Chrony and Timedatectl/systemd-timesync support

Add to the Hobbit/Xymon Plugin "ntpq" the comptatibility with "chronyd", "ntpd" should continue to work (not tested so far)

Tested on debian 11,12 chrony v4.0

How to install 
- Install Xymon Client (should have already): apt install xymon-client
- Install Xymon apt and other plugin (if not already):apt install hobbit-plugins
- Replace original (/usr/lib/xymon/client/ext/apt but it could be erased with an update...that is what I do for now) or ???

![image](https://user-images.githubusercontent.com/8841264/174496845-0e96330f-13a1-4e00-aa81-d1544ceaa891.png)

Credit to Sylvain MAURIN for timedatectl/systemd-timesync
