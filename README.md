# MyLearningNotes

## Git

____
## CMake
* https://shot511.github.io/2018-05-29-how-to-setup-opengl-project-with-cmake/ (Set up OpenGL project with CMake with prerequisites GLAD/GLFW3/GLM/stb_image)
____
## C/C++

____

## Linux
### Software update(Ubuntu)
```
apt list --upgradable  # To see available updates
sudo apt-get update    # Get updated software list for Ubuntu
sudo apt-get upgrade   # Update software(s) i.e. apply updates and patches on Ubuntu Linux
```
Please note that above two commands will fetch files from the Internets or local mirrors. The location of update pages is specified in /etc/apt/sources.list (repositories). You need NOT to make any changes to this file until and unless you need extra repositories for your setup.

### Install kernel updates on a Ubuntu LTS server
```
sudo apt-get dist-upgrade
sudo reboot  # reboot the Linux server, if a new kernel installed
```

### Install build-essential
```
sudo apt update # get update first!
sudo apt install build-essential
```
It will be a good idea to run the autoremove command to remove the residual dependency packages
```
sudo apt autoremove
```
____
## Useful tools
### system tools:
* TreeSize - windows store
* Rapid Environment Editor
* Greenshot

### dev tools:
* WinMerge
* MSYS2
* Python
* VS Code
* CMake
* Git
* yEd
* Source Trail
