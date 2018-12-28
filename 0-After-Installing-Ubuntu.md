## Decrease Swap Use
**************************

Check swappiness here:

```
cat /proc/sys/vm/swappiness
```

Default value is 60. Change it to: 10

```
sudo vim /etc/systemctl.conf
```

Add the following line to it.

```
vm.swappiness=10
```

Save the file and reboot the system to let the new value takes in effect.

## Enable Drive Cache

Go to menu and open "Disks" application. From the Left sidebar, select your primary Disk on which Ubuntu is installed. From the top menu bar, click on the Options button and select "Drive Settings...". Click the "Write Cache" tab and enable write cache setting.

