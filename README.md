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

# License
The MIT License (MIT)

Copyright (c) 2015 FarmBot

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
