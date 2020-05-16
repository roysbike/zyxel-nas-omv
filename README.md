# zyxel-nas-omv
Install Openmediavault on Zyxel NAS 520/540/542
Устнаовка Openmediavault на сетевое хранилище Zyxel NAS 520/540/542

# Requirements
To do this we need the following things:

- a really small USB stick (or an SD card that you can trust)
- A Zyxel NAS 520 or NAS 540 or NAS 542

On Windows:
 - Putty
 - Win32 Disk Imager
 
 On MacOS/Linux
 - Terminal
 - DD util
 
 
 
 # Write the image to a USB stick
 Prepare stick: Linux
Here board means are enough and you can write the image on the stick via DD.

Unzip the downloaded image:

<code>
gunzip debian-nas-stretch-18.069-armhf.img.gz
</code>

Find out which drive the USB stick is:

<code>
diskutil list
</code>

Write the extracted image on the stick with DD:
<code>
sudo dd  if=/Users/roys/Downloads/nas542/debian-nas-stretch-18.069-armhf.img of=/dev/rdisk2  bs=4m
</code>


