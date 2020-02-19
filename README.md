# Message-Transreciving-using-Mobile-Ad-Hoc-Network-MANET-

This project is visioned to provide a backup radio tower when all fails during any natural disaster where it can be used to communicate with people remotely using this network.

Lets get Started.

Step 1: Enable your SSH Mode in you Raspberry Pi.


Step 2: Now Enable Ad-Hoc mode in your Pi.

sudo nano /etc/network/interfaces

auto lo

iface lo inet loopback

iface eth0 inet dhcp
 
auto wlan0

iface wlan0 inet static

  address 192.168.1.1
  
  netmask 255.255.255.0
  
  wireless-channel 1
  
  wireless-essid MANET
  
  wireless-mode ad-hoc
