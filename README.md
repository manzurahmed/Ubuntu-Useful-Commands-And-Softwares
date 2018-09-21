# Ubuntu-Useful-Commands

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
