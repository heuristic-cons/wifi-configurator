# About
This program provides you with a simple way to configure wifi enabled linux devices to connect to a wifi network. Why? Because a lot of devices such as the Raspberry Pi or Beagle Bone require the use of a keyboard and monitor plugged into the device, or SSHing into over ethernet just to edit the config files that allow it to connect to a network. This is a pain to do for many devices, and we think it can be a lot easier for you if you use this program!

# Wifi Configurator Flow
1) Device boots up, and so does the 'wifi configurator' program

2) The program looks for a config file in a specific location, but there will not be one yet

3) Because there is no file, the device does not know which network to connect to (SSID) or the password

4) The device will then create its own wifi network, called for example: 'FarmBot Wifi'

5) The user connects to this network using their phone or laptop and opens the web browser to any URL

6) By using a captive portal (like at hotels), every web page will redirect to the wifi configurator page (mockup below)

7) The user fills out the fields including at the minimum: one network's SSID and password.

8) The user saves and reboots the configurator program. The values are saved in a config file as mentioned in Step 2

9) The device turns off its own wifi network and attempts to connect to one of the networks in the config file

10) If successful, success!

11) If unsuccessful after a minute or so, turn on 'FarmBot Wifi' again

12) If a connection is ever lost, turn on 'FarmBot Wifi' again (in case the user changes their router or moves the device's location or something)
