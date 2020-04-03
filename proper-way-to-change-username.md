#Proper way to change username

One solution could be, logoff and relogin as **root**.

```
useradd -m newusername
passwd newusername
cp -R /home/oldusername/* /home/newusername
chown -R newusername /home/newusername
```

Logoff and login as newusername.
if everything is to your satisfaction, you can remove your oldusername.

