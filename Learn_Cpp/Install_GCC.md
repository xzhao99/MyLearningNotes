#### Installing GCC on Ubuntu 20.04
The default Ubuntu repositories contain a meta-package named “build-essential” that includes the GNU compiler collection, GNU debugger, and other development libraries and tools required for compiling software.

To install the Development Tools packages, run the following command as root 
```
sudo apt update
sudo apt install build-essential
```
The command installs a lot of packages, including gcc, g++ and make
______

#### install multi-version of gcc/g++/gfortran, e.g. version 11 on Ubuntu 20.04
Run the following command to add the Toolchain repository:

```
sudo add-apt-repository -y ppa:ubuntu-toolchain-r/test
```

Install gcc 11:
```
sudo apt install -y gcc-11 g++-11 gfortran-11
```
Check gcc version to verify that the installation completed successfully:
```
gcc-11 --version
g++-11 --version
gfortran-11 --version
```
The commands below configures alternative for each version and associate a priority with it. The default version is the one with the highest priority:
```
sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-11 110 --slave /usr/bin/g++ g++ /usr/bin/g++-11 --slave /usr/bin/gcov gcov /usr/bin/gcov-11
sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-10 100 --slave /usr/bin/g++ g++ /usr/bin/g++-10 --slave /usr/bin/gcov gcov /usr/bin/gcov-10
sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-9 90 --slave /usr/bin/g++ g++ /usr/bin/g++-9 --slave /usr/bin/gcov gcov /usr/bin/gcov-9
sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-8 80 --slave /usr/bin/g++ g++ /usr/bin/g++-8 --slave /usr/bin/gcov gcov /usr/bin/gcov-8
```
Later if you want to change the default version use the update-alternatives command:
```
sudo update-alternatives --config gcc
```
You will be presented with a list of all installed GCC versions on your Ubuntu system. Enter the number of the version you want to be used as a default and press Enter. The command will create symbolic links to the specific versions of GCC and G++




Testing gcc
Create a main.c file:
```
nano main.c
```
Add the following code:
```
#include <stdio.h>

int main() {
    printf("Hello world\n");
    return 0;
}
```

Compile a code:
```
gcc-11 main.c -o test
```
Run a program:
```
./test
```

#### Uninstall gcc
If you want to completely remove gcc and related dependencies, run the following command:
```
sudo apt purge --autoremove -y gcc-11 OR g++-11 gfortran-11
```
Remove GPG key and repository:
```
sudo rm -rf /etc/apt/trusted.gpg.d/ubuntu-toolchain-r_ubuntu_test.gpg
sudo rm -rf /etc/apt/sources.list.d/ubuntu-toolchain-r-ubuntu-test-focal.list
```

___________
#### Reference:
* https://linuxize.com/post/how-to-install-gcc-on-ubuntu-20-04/
* https://lindevs.com/install-gcc-on-ubuntu/
