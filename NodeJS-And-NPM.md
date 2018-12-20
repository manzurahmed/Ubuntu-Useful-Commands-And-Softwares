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
