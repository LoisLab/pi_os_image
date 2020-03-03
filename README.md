# pi_os_image
Our in-house Raspbian build that advertises its own wireless access point, and has the cloud9 web-based development environment preinstalled for easy python development through a web browser.

Download the image [here](https://drive.google.com/file/d/11INcH4EU1vZ6tqbRKVsq9-0XMmLCJBnF/view?usp=sharing)

To use:
- Download the file
- Burn to a 16GB or larger SD card using dd or an app like Balena etcher
- Boot the Pi with the newly created SD card
- Allow the pi to boot, expand the OS, and reboot (takes a few minutes)

To connect:
- you should see a new wireless access point show up named "loislabpi-x" show up in your available networks.  
- connect to it using a password of "loislabloislab".
- open a web browser and go to http://192.168.4.1:8000 and log in as "loislab" with a password of "loislab"

Through the web interface, you can create or edit python code files, and access a terminal (bash) shell to manage the raspberry pi.  

Please note that SSH is also enabled, if you wish to use that.

Also note that this information (including passwords) is available on the public internet, so either change these passwords or assume your pi isn't secure. 

Take a look in /etc/hostname, /etc/hostapd/hostapd.conf, and /etc/network/interfaces if you want to customize/configure the wireless AP behavior, uplink it to your existing wireless network, or change the device hostname.  This is really handy if you need to deploy 30 of these in a classroom.  :)

Enjoy,
jeff@loislab.org
