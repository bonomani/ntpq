# ntpq
The Xymon script monitors ntpd, chrony, and timedatectl/systemd-timesyncd to assess NTP synchronization status, providing detailed metrics like Offset, Delay, and Jitter. 
It supports configurable warning and critical thresholds, integrates seamlessly with Xymon for status reporting, and ensures compatibility across varied system setups by dynamically detecting and adapting to the available NTP service
- Credit to Sylvain Maurin for then Timedatectl implementation 
- Credit to Peter Eisentraut for the NTPd implementation

Tested on debian 11,12 chrony v4.0
- Last Update 25.01.2025: 
  - Restructure the code to make it easier to maintain
  - Improve the chrony parts

How to install 
- Install Xymon Client (should have already): apt install xymon-client
- Install Xymon ntpq and other plugin (if not already):apt install hobbit-plugins
- Replace original (/usr/lib/xymon/client/ext/ntpq but it could be erased with an update...that is what I do for now) or ???
- (Optional: Use [xymonbody](https://github.com/bonomani/xymonbody.css) for better icon alignment)

![ntpq-chronyd](https://github.com/user-attachments/assets/6dbc8dca-07f0-4869-af00-0d67a9c42eab)
