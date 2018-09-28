## Where are all the major log files located?

All log files are located in **/var/log** directory. In that directory, there are specific files for each type of logs.

For example, system logs, such as kernel activities are logged in **syslog** file.

Some of the most common log files in that directory is :

- In directory **apt** there is a file **history.log** which saves all the package installation and removal information even the initial system build as Live CD. You can open this file to see this very interesting file.

- In directory **dist-upgrade** there is a file **apt.log** which logs the information during distribution upgrades

- In directory **installer** the log files which are created during installation can be found.

- There is an **apport.log** file which saves information about crashes in your system and reporting them.

- The file **auth.log** includes information about the authentication activities such as when you authenticate as root user via sudo.

- The file **dpkg.log** saves the low level details of package installation and removal related with **dpkg**. You might be aware that the **apt** system depends on **dpkg** for package installation and removal.

- **boot.log** includes information of each booting.

- **kern.log** saves kernel information such as warnings, errors etc.

- **alternatives.log** includes the history of all the alternatives set by various packages and their removal via **update-alternatives** command.

- Another important log file is **Xorg.log** which include information about the graphics driver, its failures, warnings etc.

Some other types of Log files may be there depending on your installed packages. For example, My system also includes a log files epoptes.log which will only be there if you install epoptes package.

### Changes after systemd

With the advent of **systemd**, logging is mostly handled by **journalctl** utility and store the logs in binary format in **/var/lib/systemd/catalog/database** file. This file enumerates all logs including kernel, boot and application logs and provides required logs via **journalctl** utility.

Here is a good article on **journalctl** on how you can use it to fetch required log info.

https://www.digitalocean.com/community/tutorials/how-to-use-journalctl-to-view-and-manipulate-systemd-logs#setting-the-system-time

