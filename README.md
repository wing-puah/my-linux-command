# My linux command
Work in progress...

__My distro: Ubuntu 18.04 LTS__

## Basic command
_(Suppose one day, I lost my memory on all things linux)_

Command | Uses
---|---
: > fileToClear | Empty file content
cat /local/directory | Short for 'concatenate'. Display contents of file
cat file1 file2 | View contents of multiple file
cat > new_file1 | Create a file
cat file1 > file2 | Redirect standard output of file into a new file else existing file. Existing contents of file2 will be overwritten by contents of file1 content
cat file1 >> file2 | Append content of file1 at the end of file2
cat file1 file2 file3 > file4 | Create a file called file4 with all output from file1, file2 and file3
cd | Change directory
cp source_file destination_file | Copy files from source file to destination file
clear | Clear the screen
grep <something> | Search for matches
kill | Kill a process
ls | List
mkdir | Make directory
mv | Move or rename (Be careful with this command, I once wipe out my user because of this command)  
ps aux | See the processes running in the system (good for kill)
rm | Remove file
rm -rf | Remove -Recursive -Force. Remove every folder, file and directory within the specified directory/folder
rmdir | Remove directory
scp source_file user@destination_host:destination_folder | Secure copy source file from server to destination folder at destination host
scp -r source_folder user@destination_host:destination_folder | Secure copy source folder
ssh-keygen | Generate new SSH keys (Default SSH directory is ~/.ssh)
ssh user@serverip | Secure shell
top | CLI interface to monitor processes and system resources usage
touch | Make file
--version | Show file version


## LAMP
### Apache
`sudo apt-get install apache2`

*When everything screws up very badly and you want to clear everything to a true clean state.*

`sudo apt-get remove --purge apache2`

`whereis apache2` OR `which apache2`

__delete the file shown in the above command__

### MySQL
`sudo apt-get install mysql-server`

### PHP
```console
sudo apt-get install php7.1
sudo apt-get install libapache2-mod-php5
```

### Start/Restart/Stop Server
`sudo /etc/init.d/apache2 start`

`sudo /etc/init.d/apache2 restart`

`sudo /etc/init.d/apache2 stop`


## Python
### Virtualenv
__Install__

`pip install virtualenv`

__Create a virtual environemnt__

```
cd my_project_folder
virtualenv my_project
```

__Activate the virtual environment__

`source my_project/bin/activate`

*Name of the current virtual environment will appear on the left of the prompt (e.g. (my_project)Your-Computer-Name:your_project UserName$*

__Deactivate the virtual environment__

`deactivate`

## RaspberryPi
__Find Raspi IP__

`ping raspberrypi.local`

__Passwordless SSH access__

`cat ~/.ssh/id_rsa.pub | ssh user@raspiIP 'cat >> .ssh/authorized_keys'`

__Reboot__

`sudo shutdown -r now`

__Shutdown__

`sudo shutdown -h now`
