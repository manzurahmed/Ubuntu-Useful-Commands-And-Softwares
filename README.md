# Ubuntu Useful Commands And Softwares


### List of Softwares

- Pick - A colour picker for Ubuntu, elementary, and other Linux OSes: https://kryogenix.org/code/pick/
- FileZilla for Ubuntu: https://filezilla-project.org/download.php?platform=linux
- SSH: Putty:

  ```
  $ sudo apt-get update
  $ sudo apt-get install -y putty
  ```

- Koala - Less, Sass, Compass and CoffeeScript compilation: http://koala-app.com/
- Zeal Docs - Offline documentation: https://zealdocs.org/
- GIMP Image manipulation: https://www.gimp.org/downloads/
- Vector Image Manipulation: Inkspace: https://inkscape.org/en/
- LibreOffice - Microsoft Office alternative: https://www.libreoffice.org/
- Visual Studio Code on Linux: https://code.visualstudio.com/docs/setup/linux
- Image Viewer: xnView: https://www.xnview.com/en/xnviewmp/#downloads
- Google Chrome: https://google-chrome.en.uptodown.com/ubuntu
- Firefox Quantum: Always install from "Ubuntu Software"
- Download Manager: uGet: https://ugetdm.com/
- Remote Desktop - AnyDesk: https://anydesk.com/platforms/linux
- Bangla Keyboard: Avro Keyboard
   #### How to install:
   1. http://linux.omicronlab.com/
   2. https://www.youtube.com/watch?v=0jYQZ6PSpbs
   3. https://ottopor.com/en/it/unijoy-layout-in-ubuntu-gnome-17/

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

## Google Chrome

- Go to https://www.google.com/chrome. Click the Download Chrome button.
- Then select the first option (64 bit .deb for Debian/Ubuntu), click Accept and Install.
- When Firefox asks you how to open this deb file, choose the default option to open it in Ubuntu Software (formerly Ubuntu Software Center).
- If you choose the first option, Google Chrome deb package will be downloaded to /tmp/mozilla_$username directory. Once the download is complete, Ubuntu Software will automatically open. Click the Install button to install google-chrome-stable to Ubuntu 18.04.
- Because software installation on Linux requires root privilege, so you have to enter your password to authenticate.

Once the installation is complete, you can start Chrome browser from applications menu

## DU Meter

Open "Ubuntu Software", type "netspeed" and press the Enter key. Follow instructions to finish installation.
