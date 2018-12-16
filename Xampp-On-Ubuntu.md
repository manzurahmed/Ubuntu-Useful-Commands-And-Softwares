# How to install Xampp 7.2.4 on Ubuntu 18.04

**Follow this Video tutorials**
1. https://www.youtube.com/watch?v=a0VPzhOG3YM
2. https://www.linuxhelp.com/how-to-install-xampp-7-2-4-on-ubuntu-18-04

## Steps

### Download Xampp
```
wget https://www.apachefriends.org/xampp-files/7.2.12/xampp-linux-x64-7.2.12-0-installer.run
```

### Give the execution permission for downloaded xampp file

```
chmod +x xampp-linux-x64-7.2.4-0-installer.run
sudo ./xampp-linux-x64-7.2.4-0-installer.run
```

## WORDPRESS ASKING FOR LOCAL FTP CREDENTIALS ON XAMPP
```
$ cd /opt/lampp
$ sudo chown -R daemon htdocs
$ sudo chmod -R g+w htdocs
```

### More on Permission

https://unix.stackexchange.com/questions/276142/touch-cannot-touch-test-permission-denied
https://www.computernetworkingnotes.com/ubuntu-linux-tutorials/how-to-fix-permission-of-htdocs-folder-in-ubuntu-linux.html

https://www.computernetworkingnotes.com/ubuntu-linux-tutorials/how-to-start-xampp-automatically-in-ubuntu-linux.html

## How to start XAMPP Automatically in Ubuntu Linux

Since XAMPP is the third party software, Ubuntu does not start it in boot process. Before we use it, we have to start it manually with following command to start Xampp manually.

```
sudo /opt/lampp/lampp start
```

### Creating a script to stat XAMPP automatically

```
sudo vi /etc/init.d/lampp
```

```
#!/bin/bash
### BEGIN INIT INFO
# Provides: lampp
# Required-Start:    $local_fs $syslog $remote_fs dbus
# Required-Stop:     $local_fs $syslog $remote_fs
# Default-Start:     2 3 4 5
# Default-Stop:      0 1 6
# Short-Description: Start lampp
### END INIT INFO
/opt/lampp/lampp start
```

Save the file. Then run the following command:

```
sudo chmod +x /etc/init.d/lampp
```

Then, run the following command:

```
sudo update-rc.d lampp defaults
```

### Testing

```
systemctl list-units --type service |grep lampp
```

XAMPP uses lampp service to control all its operation in Ubuntu.

We can also verify the starting of XAMPP by accessing following URL in web browser

```
http://localhost
```
