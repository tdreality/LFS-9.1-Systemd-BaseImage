# LFS-9.1-Systemd-BaseImage

What a built Linux From Scratch (LFS) machine looks like at its base (Without BLFS and user interface).

### What's the purpose of this?
The purpose of uploading this built LFS image is for other people to check what a base LFS image would look like in case they are thinking of trying out LFS themselves. I hope people are not put off by the simplicity of an LFS image although there were some parts that were quite challenging for me and took me more than a week and a couple of rebuilds. I hope this encourages people to try LFS and build their own Linux OS. I'd say LFS is a great learning opportunity and I do certainly understand Linux more now compared to before because of this.

About the image being a plain LFS, well, not purely as it does contain a little BLFS in it such as the *mkinitramfs* script and *cpio-2.13, LVM2-2.03.08* and *mdadm-4.1* packages. I needed the *mkinitramfs* for booting the kernel in some cases and it required the *cpio-2.13* package for making the *initrd.img*

This build uses the Linux kernel version 5.5.3 and uses Systemd instead of Sysvinit.

## Guide used
http://www.linuxfromscratch.org/lfs/view/stable-systemd/

## Image download URL:
https://github.com/tdreality/LFS-9.1-Systemd-BaseImage/releases

## How to boot
* VMware
  * Simply import the OVF file and run
* VirtualBox
  * Create a **New** VM
  * Type: **Linux**
  * Version: **Linux 2.6 / 3.x / 4.x (64-bit)** or **Other Linux (64-bit)**
  * Choose the **Use an existing virtual hard disk file** and select the .vmdk file included in the download

In case of kernel booting issues, make sure the Disk Type chosen is "SATA"
  
  
Username | Password
------------ | -------------
root | user@123

