## Install JDK 8

Tutorial: https://linuxconfig.org/install-android-studio-on-ubuntu-18-04-bionic-beaver-Linux

### Add PPA

Using Webupd8 Team's PPA repository we can install Java on Ubuntu automatically using the apt command. Webupd8 Team currently maintains Oracle Java 8 and Oracle Java 9 PPA repositories for Ubuntu 18.04 Bionic Beaver. 

```
$ sudo add-apt-repository ppa:webupd8team/java
$ sudo apt update
```

### Install Java on Ubuntu

After adding PPA repository we can move to installing java on Ubuntu. Executing apt search oracle-java command should now show multiple java versions available for install.

Namely they are java8 and java9.

#### To install Java 8 execute:

```
$ sudo apt install oracle-java8-set-default
```

The above commands will automatically install selected java version and set all necessary java environment variables. 

```
$ java -version
java version "1.8.0_181"
Java(TM) SE Runtime Environment (build 1.8.0_181-b13)
Java HotSpot(TM) 64-Bit Server VM (build 25.181-b13, mixed mode)
```
