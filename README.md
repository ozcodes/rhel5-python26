# rhel5-python26
Installing Python 2.6 on RHEL 5

Instructions:
-------------
Get the epel-release-5-4.noarch.rpm from fedora archives at:
https://archive.fedoraproject.org/pub/archive/epel/5/x86_64/epel-release-5-4.noarch.rpm

Place the file in the root directory of the machine
Start install.sh script

Additional info
---------------
The script install the epel file in order to use yum for the python 2.6 installation and then add python 2.6 as an alias to the python command so that when python is used it uses the python 2.6 and not the 2.4 that comes with fresh install of rhel.

Python 2.6 as permenent default python
--------------------------------------
You will notice that after reboot python 2.6 is not the default python.
To make it so insert this line "alias python='/usr/bin/python2.6'" in the user's ".bashrc" file. for example if you use root as your user the file would be at /root/.bashrc
