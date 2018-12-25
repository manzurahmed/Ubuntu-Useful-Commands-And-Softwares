I have used a tutorial from FossBytes website to learn about creating bootable USB stick in Ubuntu. Normally, I used Rufus in Windows, but, it is not available in Linus platform. 

https://fossbytes.com/create-bootable-usb-media-from-iso-ubuntu/

# Convert ISO to USB in Ubuntu Using ddrescue

Well, hang on. This is Ubuntu we are talking about. Apparently, the terminal is the top tool for a typical Linux user. So let’s just say that we were saving the best for the last. This is by far the easiest way to convert ISO files to a USB disk if you are fond of using terminal commands.

For starters, ddrescue is a data recovery tool which can clone any storage devices. We can use ddrescue to convert ISO files to USB sticks.
Install ddrescue

First things first. You will need a working internet connection to download and install ddrescue. (In case you already have it installed, you can skip this step).
```
sudo apt update
sudo apt install gddrescue
```
Now, you will need to know the exact block device name (something like dev/sd..). To do this use the command fdisk. Enter the following command,
```
sudo fdisk -l
```
Once you enter the fdisk command, you can see all your devices connected. Here, you can see that the block device name for the USB is /dev/sdb1.

Importantly, verify that the block device name you chose is the correct one or you might end up with corrupt/destroyed data.

Once done, enter the command as follows:

```
ddrescue path/to/.iso /dev/sdx --force -D
```

Replace the **x** and **path/to/.iso** with your specific device block name and the path for the iso file.

When the process is finished, you can boot into your bootable Ubuntu USB stick.
