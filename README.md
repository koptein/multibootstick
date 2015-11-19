#Installation
You need an USB stick with at least 4GB Space, 8GB are recommended.

Partition and format the whole Stick to a single FAT32 Partition with activated boot flag. (gparted or fdsik will do the trick)
Unzip the multiboot files to the stick and install grub to the usbstick:
<pre><code>
mount /dev/sdX1 /mnt 
tar xfvz /path/to/file/multibootstick_v0.2.tar.gz -C /mnt
grub-install --target=i386-pc --recheck --boot-directory=/mnt/boot /dev/sdX
</pre></code>
