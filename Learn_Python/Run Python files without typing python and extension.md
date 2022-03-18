## How to run python files without typing python and extension (in Linux)
Watch the video here https://www.youtube.com/watch?v=5CMmjNt_p48
Steps to follow to run your python code without typing python filename.py.

You can simply run by typing *filename* if you follow these simple steps.

### Step 1 : Add shebang line as first line in your python code
```
#!/usr/bin/python3
```
This line tells about the location of interpreter.

If you are using another version of python, find that interpreter and type it in here. (I am having two version of python, python 2.7 and python 3.5 and to run it with python3 interpreter we have to type in ```/usr/bin/python3```)

If you are using virtualenv, you can simply modify the shebang line to your interpreter.

### Step 2 : Make your python file executable
In terminal, go to your directory where your python file is located and type the below command.
```
chmod +x filename.py  # make the file executable
```
For example we have hello.py as our file, so we will move to the directory where it is located and will do
```
chmod +x hello.py
```
Now you can run your python file like ./hello.py

### Step 3 : Move your file to bin to run it from anywhere
In terminal type the following command
```
cp filename.py ~/bin/new_name_you want_to_run_with
```
For example I want to run this file by calling welcome, I will do
```
cp hello.py ~/bin/welcome
```
Now you can run this welcome from anywhere on your system by just typing welcome in terminal.

### A few improvements:

The following shebang line is better, because it will also work with virtual environments.
#!/usr/bin/env python

Hard-wiring the path of the Python interpreter is prone to breaking.

Instead of creating a copy of the script under a new name, I would recommend creating an alias, e.g. in ~/.bash_profile (OSX) or ~/.bashrc (Linux), like so
alias python_example='python_example.py'

This works like a charm and will always call the latest version of the script.
________________________

### Reference:
https://gist.github.com/umangahuja1/51da3a453803f1f67f4eee5de129d4db
