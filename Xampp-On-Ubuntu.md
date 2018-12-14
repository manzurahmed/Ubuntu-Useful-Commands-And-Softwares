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
