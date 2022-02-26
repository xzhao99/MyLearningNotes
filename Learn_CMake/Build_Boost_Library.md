# Build Boost Library under WSL

## Instructions:

https://github.com/boostorg/wiki/wiki/Getting-Started%3A-Overview

### git clone --recursive https://github.com/boostorg/boost.git
### cd boost
### git checkout develop # or whatever branch you want to use
### ./bootstrap.sh --help # see what options we can define

### ./bootstrap.sh --prefix=/home/xzhao/workdir/boost/ --with-libraries=all
### ./b2
### ./b2 headers

### **Message:**
...updated 1602 targets...


The Boost C++ Libraries were successfully built!

The following directory should be added to compiler include paths:

    /home/xzhao/workdir/boost_git_src

The following directory should be added to linker library paths:

    /home/xzhao/workdir/boost_git_src/stage/lib
