directory 

4.2.1 build Linux virtual machine 

4.2.2 command line in Linux 

Common commands in 4.2.3 Linux 

4.2.4 Linux environment variables PATH 

4.2.5 system to learn Python 

##  4.2.1 build Linux virtual machine 

When developing in the enterprise, the Linux system is usually used as the server, and it is necessary for readers to master the basic knowledge of the Linux system first. To operate in the Linux, it is mainly through the command line in the end point. Before that, readers need to set up Linux learning environment. 

In this section, the author teaches students how to create Linux virtual machine in Windows system. 

Follow these steps to create Linux virtual machine: 

(1) Install VMware Workstation Player 

Download the latest version of VMWare Workstation Player from VMware's official website: 

下载 VMware Workstation Player | VMware | CN 

After downloading to the local area and installing it successfully, click the icon of VMware Workstation Player on the desktop, and the following window will appear: 

![avatar]( 91a5c20071c37992d3589e8f63055f95.png) 

In the toolbar on the right side of the window, there are four menus in total. Click the "Create New Virtual Machine" menu to create a virtual machine. To create a virtual machine, you need to download the image files of other systems first. Enterprises usually use CentOS systems as servers, and in this section, CentOS image files are used to create Linux virtual machines. 

(2) Download the CentOS image 

Click the link: 

http://isoredirect.centos.org/centos/8/isos/x86_64 

Go to the official download page of the CentOS image file: 

![avatar]( c27517338d8b8baca20fef20e9a1b829.png) 

Click the Alibaba Cloud link in the download link list to download. The one with aliyun in the link is the Alibaba Cloud link. 

(3) Create a virtual machine 

After downloading the image file locally, click the "Create New Virtual Machine" menu in the VMware Workstation Player window: 

![avatar]( 3b8d7725616f06b2b52f6648418a5edc.png) 

Select "Installer CD Image File", click the Browse button, select the downloaded image file, and then click Next: 

![avatar]( 4be2962bb15f9c4a06737e696013af74.png) 

Fill in the title, username and password of the Linux virtual machine in the window, and then continue to click Next: 

![avatar]( 68b1fe7e30761c064aab66278d49a5dd.png) 

Fill in the virtual machine name and installation location, and continue to click Next: 

![avatar]( e90803c2b31bde99f26faed7c3266646.png) 

Readers can configure a reasonable hard disk size according to the hardware configuration of the local machine, and then continue to click Next: 

![avatar]( d865d600ab907f657ed53f20c861e80b.png) 

Click the Finish button to start creating Linux virtual machine. 

(4) Install the virtual machine 

During the first installation, VMware Workstation Player automatically loads two image files, which can cause problems during installation. At this point, you need to shut down the virtual machine and open the VMware Workstation Playe panel to set the following settings: 

![avatar]( 096ca237bb0e2eb8b2438b8785b42136.png) 

In the home window on the left side of the panel, click the virtual machine name and right-click the "Settings" menu: 

![avatar]( 1e4c8b44cb3f3a958c6d08b8b07c2bff.png) 

Connect at startup to the right of CD/DVD (IDE) in the virtual machine settings box, uncheck: 

![avatar]( 7043a346b337616217d8f1eb773e45eb.png) 

Then click the OK button, go back to the panel and double-click the mouse on the virtual machine, and the virtual machine will automatically turn on. At the beginning of the installation, the following interface will appear. At this time, you need to click to enter the panel and select the first line through the arrow keys. After selecting, the font will turn white: 

![avatar]( b3dd0286f955c79e19d2b08b40aacb71.png) 

After selecting it, press the Enter key to start the installation of the virtual machine. During the installation process, click the "Continue" button all the way to configure the default. When the following interface appears, you need to click the Installation Destination button in the panel to configure the disk partition: 

![avatar]( 242af25f10151c38f614b09b4e2069ad.png) 

After entering, VMWare will automatically configure the disk partition, and then click the blue Done button in the panel: 

![avatar]( 1b66402344d142b4330a174a34be453a.png) 

Then click "Begin Installation" in the panel to install the virtual machine: 

![avatar]( 4a4c2ffdaef59e316d02ef2d8d2aa222.png) 

During the download process of the installation package, click Root Password to set the password of the root of the super administrator account, and click User Creation to create a new user: 

![avatar]( 4f65059bc626ea3ffddc0d3be7b40674.png) 

Students must save the login password of the root account and other accounts. When logging in to the Linux system, you need to enter the password for login verification. After the installation package is downloaded and installed successfully, the panel will restart. Check the license agreement of the CentOS system when restarting, and then click the blue Done button in the upper left corner. 

![avatar]( 51cba64760bf05c2d636a54590c94a2e.png) 

Finally, the login interface of the CentOS system will appear. 

![avatar]( 2e0e4e80f636b8eb5c747849fec65d07.png) 

Now click on the account to enter the password and start our Linux system learning journey! 

##  4.2.2 command line in Linux 

After entering the CentOS system, click the Activities menu at the top of the desktop, and a toolbar will appear on the left side of the desktop: 

![avatar]( 6c354980361d2ea580c4cffe1b95ad90.png) 

![avatar]( e8657bfedbb8b7b311fe072b8c5c82a1.png) 

Click on the end point of the arrow to enter the command line: 

![avatar]( 64eb3f9c0cd7117db12cc01a9c3eb9f5.png) 

After entering the Linux system, VMWare Workstation 15 Player may have a problem that the screen is too small and cannot be stretched.

Enter the following command on the end point command line to resolve the issue:

Execute the sudo yum install xorg-x11-drv-vmware -y command on the command line (the sudo command will ask for the password of the root account),

Then execute the shutdown -r now command to restart. 

##  Common commands in 4.2.3 Linux 

(1) Directory display: ls 

The ls command is used to display the contents of the directory. The basic syntax of the ls command is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
path_of_directory represents the path of the directory, and when the path is empty, the contents of the current directory will be displayed by default. 

Example demonstration: 

Display all files in the current directory: 

![avatar]( ad44f32be78a713ded9ab7cb529773ad.png) 

(2) View Help: man 

Linux the commands in the system provide a wealth of options. To view the definition of the command and the usage of the options, you can use the man command in the system. 

Basic usage of the man command: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
Command represents the name of the command. 

Example demonstration: 

Review the ls command's definition and option usage: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
![avatar]( 0b93bd4db735e3ed0f93c337891cc590.png) 

Press the q key on the keyboard to exit the man command. 

In the output of the man ls command, you can see the description of the ls command: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
From the description of the ls command, ls is used to display the contents of the directory. 

Linux the options in the command are mainly divided into short options and long options, with a dash symbol "-" for the short option,

Long options are those with two dashes. When command options take arguments, the arguments must follow the options. 

For example, -a in the ls command is the short option, --all is the long option. Multiple options in the command can be used together. Continuing to use the ls command as an example, it can be seen from the output of man that the --all option will display all files including the. and.. symbols (prefixed with.), and the -l option will display the author of the file. 

Example demonstration: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
![avatar]( dc680d89ec7d563edd187cc57110ce2d.png) 

(3) Directory switch: cd 

The cd command in Linux is similar to the cd command in windows, and is used to switch directories. In Linux systems, there are also two special directory symbols. and.., which represent the current directory and the parent directory respectively. Readers should note that in Linux systems, the separator between directories is "/". 

Linux system does not have the concept of disk letters, in Linux system everything is a file, directory is also a file, all files with "/" as the root directory. 

Basic usage of the cd command: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
Parameter path_of_directory represents the path of the directory, when the directory is empty, it will automatically switch to the current user's home directory. 

The path to the home directory is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
Username represents the login username. For example, if the author's login username is chipscoco, then the home directory is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
Example demonstration: 

Switch to home directory: 

![avatar]( 8b77f85ae6b4b541c0bf1675202255d8.png) 

Switch to the home directory as a directory path: 

cd /home/chipscoco 

![avatar]( 01bc30e9423ef2fa9d8faa8767ecda8a.png) 

Linux command line also provides the function of automatic completion, when performing operations such as directory switching, pressing the TAB key of the keyboard can automatically complete the command. 

(4) Directory creation: mkdir 

The mkdir command is used to create directories. Basic usage of mkdir: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
Example demonstration: 

Create the python3-learning directory in the home directory: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
![avatar]( 09dd6571c1b2d703f3d7b1b05e757848.png) 

Directory creation is the opposite of directory deletion, using the rm command to delete files, and adding the -rf option to force deletion when the directory is not empty. 

Before deleting files, it is a good habit to maintain a file backup. 

(5) File copy: cp 

The cp command is used for copying files. The basic usage of the cp command is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
The parameter source represents the original file or directory, and dest represents the new file or directory after copying. When the directory is not empty, the -r option needs to be added. 

Example demonstration: 

![avatar]( 872c7129da3fb8a2dae9cf6be6dd09dd.png) 

In the figure, the docs directory was created in python3-learning through the mkdir python-learning/docs command respectively. Then copy the python-learning directory to the new directory python3 through the cp -r command. 

(6) File editing: vim 

Vim in the Linux system is an editor, and in the eyes of technical geeks, vim is called "the artifact in the editor". The detailed usage of the vim tool is not introduced in this book, and interested readers can learn from other materials. 

Basic usage of the vim command: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
path_of_file represents the path to the file, and a new file is created when the file does not exist. 

There are three modes in the VIM editor: 

![avatar]( 62b455335fc8fefa7fe9c9749689c5ad.jpeg) 

Example demonstration: 

Switch to the python3-learning directory and edit hellopython.py file: 

![avatar]( 42c5b91d587c7b79892f235bc1aea022.png) 

When entering the editor, you initially enter command mode. 

![avatar]( 66a9c96784f8325f03f5b6e76813e919.png) 

Press the a key of the keyboard in command mode to switch to edit mode, where you can see the INSERT prompt at the bottom: 

![avatar]( b69cddb91e5b4920e35468021f9e1ed2.png) 

Edit the file in vim: 

![avatar]( f2ad77e832afc60ab0effead5d46e743.png) 

Switch to command mode, then switch to last line mode. Enter x in last line mode to exit vim: 

![avatar]( 4ce72afd596fabecdecd1c118db685d6.png) 

(7) View files: head, tail, cat, more 

Linux the head, tail, cat, more commands can be used to view the content of the file, the content display is slightly different, head is used to display 10 lines of content starting from the file header, tail is used to display 10 lines of content starting from the end of the file, cat is used to connect multiple files and output to the screen. The more command is similar to the more command of the windows system, which is used to display the content in sections. 

Example demonstration: 

View file contents in hellopython.py: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
![avatar]( 8446c7f74abfb08d18e68f4e57b5c388.png) 

(8) System shutdown: shutdown 

System shutdown using the shutdown command: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
Use the shutdown command to restart the system: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
In this section, the basic usage of common commands in the Linux system is introduced. Learning the above commands is basically enough for beginners to cope with daily development work. 

For the detailed usage of the command, the reader can find it through the man command. For further study of the Linux system,

I recommend the book Linux Command Line and Shell Scripting. 

##  4.2.4 Linux environment variables PATH 

(1) Introduction to PATH 

Linux environment variables of the system and environment variables of the windows system, save a series of parameters of the system running environment, such as environment variables PATH, save the parameters related to the path. 

(2) Configure PATH 

Format of PATH: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
In the PATH format, paths are separated by:. 

PATH configuration syntax: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
path_of_tool represents the path to be configured. If you need to configure multiple paths, the paths must be separated by:. For example, add/home/python/bin to the environment variables PATH: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
The export command in the Linux is used to set environment variables, and the variable name is preceded by a $sign to indicate that the value of the variable is obtained. 

Use the echo command to output the value of the variable: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
![avatar]( aa442a25c1afbdfe0a0ffb4e23ccafa5.png) 

For PATH = $PATH:/path_of_tool, it can be broken down into the following two steps: 

Assuming the value of PATH is/usr/bin, then $PATH:/path_of_tool becomes 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
2. Then assign/usr/bin:/path_of_tool to the variable PATH 

Variable settings are made on the command line, only valid for the current session and no longer valid after exiting the command line or restarting the system. To permanently modify the variable settings, you can write them to the configuration file/etc/bashrc or to a .bashrc file in your home directory. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589604
 ```  
##  4.2.5  

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning 

