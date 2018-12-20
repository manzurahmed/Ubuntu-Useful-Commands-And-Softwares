# How to Install NodeJS and NPM on Ubuntu 18.04

To get this version, you can use the apt package manager. Refresh your local package index by typing:
```
sudo apt update
```
Install Node.js from the repositories:
```
sudo apt install nodejs
```
If the package in the repositories suits your needs, this is all you need to do to get set up with Node.js. In most cases, you'll also want to also install npm, the Node.js package manager. You can do this by typing:
```
sudo apt install npm
```
This will allow you to install modules and packages to use with Node.js.

Because of a conflict with another package, the executable from the Ubuntu repositories is called nodejs instead of node. Keep this in mind as you are running software.

To check which version of Node.js you have installed after these initial steps, type:
```
nodejs -v
```

# Uninstall NodeJS and NPM

To remove the distro-stable version, type the following:
```
sudo apt remove nodejs
```
This command will remove the package and retain the configuration files. These may be of use to you if you intend to install the package again at a later point. If you don’t want to save the configuration files for later use, then run the following:
```
sudo apt purge nodejs
```
This will uninstall the package and remove the configuration files associated with it.

As a final step, you can remove any unused packages that were automatically installed with the removed package:
```
sudo apt autoremove
```
