# ntpq
The Xymon script monitors ntpd, chrony, and timedatectl/systemd-timesyncd to assess NTP synchronization status, providing detailed metrics like Offset, Delay, and Jitter. 
It supports configurable warning and critical thresholds, integrates seamlessly with Xymon for status reporting, and ensures compatibility across varied system setups by dynamically detecting and adapting to the available NTP service

Tested on debian 11,12 chrony v4.0
- Last Update 25.01.2025: 
  - Restructure the code to make it easier to maintain
  - Improve the chrony parts

How to install 
- Install Xymon Client (should have already): apt install xymon-client
- Install Xymon ntpq and other plugin (if not already):apt install hobbit-plugins
- Replace original (/usr/lib/xymon/client/ext/ntpq but it could be erased with an update...that is what I do for now) or ???

![image](https://user-images.githubusercontent.com/8841264/174496845-0e96330f-13a1-4e00-aa81-d1544ceaa891.png)

Credit to Sylvain MAURIN for timedatectl/systemd-timesync
