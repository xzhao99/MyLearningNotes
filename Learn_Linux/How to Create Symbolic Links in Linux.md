To use the ```ln``` command, open a terminal window and enter the command with the following format:
```
ln [-sf] [source] [destination]
```
- By default, the ```ln``` command creates a *hard link.*
- Use the ```-s``` option to create a *soft (symbolic) link*.
- The ```-f``` option will force the command to **overwrite** a file that already exists.
- Source is the file or directory being linked to.
- Destination is the location to save the link – if this is left blank, the symlink is stored in the current working directory.

For example, create a symbolic link with:
```
ln -s test_file.txt link_file.txt
```
This creates a symbolic link (link_file.txt) that points to the test_file.txt.

To verify whether the symlink has been created, use the ```ls``` command:

![image](https://user-images.githubusercontent.com/8794047/159061976-785d472f-afbb-4e99-8ac3-bb0796281542.png)


Example:
```
ln -s /usr/bin/python3.9 /usr/bin/python
python --version  # will print: Python 3.9.*
```

