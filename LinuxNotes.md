
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
