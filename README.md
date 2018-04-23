# My linux command
Work in progress... 

__My distro: Ubuntu 16.04.4 LTS__ 

## Basic command 
_(Suppose one day, I lost my memory on all things linux)_ 

Command | Uses
---|---
cd | Change directory 
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
top | CLI interface to monitor processes and system resources usage
touch | Make file 
--version | Show file version


## LAMP 
### Apache 
sudo apt-get install apache2 

*When everything screws up very badly and you want to clear everything to a true clean state.* 

sudo apt-get remove --purge apache2*

whereis apache2 

__delete the file shown in the above command__ 

### MySQL 
sudo apt-get isntall mysql-server 


### PHP 
sudo apt-get install php5 libapache2-mod-php5 

### Start/Restart/Stop Server
sudo /etc/init.d/apache2 start

sudo /etc/init.d/apache2 restart 

sudo /etc/init.d/apache2 stop 


## Python 
### Virtualenv 
__Install__

pip install virtualenv 

__Create a virtual environemnt__ 

cd my_project_folder 

virtualenv my_project 

__Activate the virtual environment__ 

source my_project/bin/activate

*Name of the current virtual environment will appear on the left of the prompt (e.g. (my_project)Your-Computer-Name:your_project UserName$* 

__Deactivate the virtual environment__ 

deactivate 
