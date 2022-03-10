
### How do I determine my Linux version?
The uname and /etc/os-release commands are the most common methods for getting the version of Linux you're running and are available by default on *any Linux system* you run. To view the contents of the os-release file, run the following command:
```
cat /etc/os-release
```
To find out what version of the Linux kernel is running, run the following command:
```
uname -srm
```
Alternatively, the command can be run by using the longer, more descriptive, versions of the various flags:
```
uname --kernel-name --kernel-release --machine
```

### How do I determine Red Hat Enterprise Linux(RHEL) version?
* To determine RHEL version, type:
```
cat /etc/redhat-release
```

* Execute command to find RHEL version:
```
more /etc/issue
```

* Show RHEL version using command line, run:
```
less /etc/os-release
```

* Another option to get Red Hat Enterprise Linux version:
```
less /etc/system-release-cpe
```

* RHEL 7.x or above user can use the  command to get RHEL version
```
hostnamectl
```

### How to update software on Linux(Ubuntu)
* Software update(Ubuntu)
```
apt list --upgradable  # To see available updates
sudo apt-get update    # Get updated software list for Ubuntu
sudo apt-get upgrade   # Update software(s) i.e. apply updates and patches on Ubuntu Linux
```
Please note that above two commands will fetch files from the Internets or local mirrors. The location of update pages is specified in /etc/apt/sources.list (repositories). You need NOT to make any changes to this file until and unless you need extra repositories for your setup.

* Install kernel updates on a Ubuntu LTS server
```
sudo apt-get dist-upgrade
sudo reboot  # reboot the Linux server, if a new kernel installed
```

* Install build-essential(gcc/make and other dev tools on Ubuntu)
```
sudo apt update # get update first!
sudo apt install build-essential
```
It will be a good idea to run the autoremove command to remove the residual dependency packages
```
sudo apt autoremove
```
