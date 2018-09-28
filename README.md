# Ubuntu Useful Commands And Softwares



### List of Softwares

1. Pick - A colour picker for Ubuntu, elementary, and other Linux OSes: https://kryogenix.org/code/pick/
2. FileZilla for Ubuntu: https://filezilla-project.org/download.php?platform=linux
3. Putty:

  ```
  $ sudo apt-get update
  $ sudo apt-get install -y putty
  ```
4. Koala - Less, Sass, Compass and CoffeeScript compilation: http://koala-app.com/
5. Zeal - Offline documentation: https://zealdocs.org/
6. GIMP - Image manipulation software
7. LibreOffice - Microsoft Office alternative
8. Visual Studio Code on Linux: https://code.visualstudio.com/docs/setup/linux
9. Image Viewer:
  - xnView
  - nomacs

### Faster app menu in Ubuntu 18.04

The link shows you how to turn off all kind of animations especially the spreading icons on menu, searching, and window animations so you can work faster. To do it, just run this command:

```
$ gsettings set org.gnome.desktop.interface enable-animations false
```

Then apply it by pressing **Alt+F2** and type **r** and press **Enter**. This will reset the GNOME Shell to follow your command.

To revert it back (enable animation again), just change the command to:

```
$ gsettings set org.gnome.desktop.interface enable-animations true
```

## Install Wine

```
$ sudo apt install wine64
```

Check your version once the Wine installation is complete: 

```
$ wine --version
```

## Xtreme Download Manager Updated With Fresh GUI

Download XDM .zip file from this link https://sourceforge.net/projects/xdman/files/ on the Desktop. Extract it by double-clicking on it. Open terminal. Navigate to the User's Desktop and further navigate to the "xdm-2018-x64" folder.

Type the following command in Terminal and press Enter key:

```
sudo ./install.sh
```

**Uninstall:**

The software offers an uninstall script in the installation directory. Simply open terminal (Ctrl+Alt+T) and run command to remove the software:
```
sudo /opt/xdman/uninstall.sh
```

## Install and Uninstall Koala

Download the 64-bit .deb package from Koala's official website: http://koala-app.com/. Double-click the .deb package file to start the automated installer. Finish installation.

**Uninstall Koala**
```
sudo dpkg -r koala
```

