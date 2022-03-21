Sharing what worked for me. Worked for me on Enterprise RHEL 7.
```
#-> python --version
Python 2.7.5

#-> yum install rh-python38

#-> scl enable rh-python38 bash

#-> python --version
Python 3.8.0
```
But you will have enter into the scl shell everytime as the default shell would still be Python 2.7. To make this permanent, I had to
```
Add this to my ~/.bash_profile

source /opt/rh/rh-python38/enable
```

**This works on brl-sim01 RHEL 7.9**
