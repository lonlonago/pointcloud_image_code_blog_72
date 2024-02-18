directory 

4.1.1 what the command line is 

4.1.2 enter the Windows command line 

4.1.3 common commands in Windows 

4.1.4 Windows environment variables PATH 

4.1.5 system to learn Python 

##  4.1.1 What is the command line? 

The command line, also known as the command prompt, is a tool provided by the operating system that can directly execute commands. In the command line interface, you can see a blinking underscore input prompt, "prompting" you to enter commands. The command line interface in Windows: 

![avatar]( 4f9f1044bc18ff034df0191701f747ec.png) 

##  4.1.2 enter the windows command line 

The cmd command is a command-line program in the windows system. In the windows10 system, press the windows key on the keyboard, and then directly enter cmd. The system will automatically match the command prompt tool: 

![avatar]( 09e12c28d51252cc4dcb8989003a3c48.png) 

Pressing the enter key will bring up the Windows command-line window: 

![avatar]( 9433d0b9ad7832d99d8aa6267b44ab79.png) 

In the command line window, you can execute commands from the system. 

##  4.1.3 common commands in Windows 

(1) cd: switch directory 

CD means "change directory" in English, which translates to switch directory. 

In Windows, directories are separated by the "\" symbol, such as the B directory in the A directory, which can be expressed as A\ B.

The. symbol and the.. symbol are special directory symbols in the system. The. symbol represents the current directory and the. symbol represents the parent directory.

The Windows system has the concept of a drive letter, which is the identifier of the disk device. For example, the drive letter of the C disk is C:, and the drive letter of the D disk is D:.

Enter the drive letter on the command line to switch directly to another disk.

In windows, directory switching can only be performed within the drive letter, and it cannot be directly switched to directories in other drive letters.

To switch to a directory with another drive letter, you need to switch between drive letters first. 

The basic syntax of the cd command: 

cd directory 

The directory parameter represents the directory name to be switched. 

Example demonstration: 

Switch from the C drive to the python3-learning directory of the D drive on the command line: 

![avatar]( 0073061c7c1c05f88999de98fee963ac.png) 

In the picture above, first enter the drive letter d: to switch to the D drive, and then execute the "cd python3-learning" command to switch to the python3-learning directory. Switch to the parent directory of the python3-learning directory: 

![avatar]( ea8be0d1b0951ed2ce4e528170539f5a.png) 

The.. symbol indicates the parent directory, and directly cd.. can be switched to the parent directory of the current directory. 

When switching directories or executing other commands, there is no need to type out the full path name, press the TAB key of the keyboard, and the system will automatically complete it.

For example, when switching to the python3-learning directory on the D disk, just enter cd python3 and press the TAB key, and the system will automatically complete it as

cd python3-learning。 

(2) dir: view directory 

Execute the dir command to view the files and subdirectories in the directory. The basic syntax of the dir command: 

dir directory 

Directory represents the directory name in the system. When the parameter directory is empty, it indicates that the files and subdirectories in the current directory are viewed. 

Example demonstration: 

Check the files in the python3-learning directory: 

![avatar]( 9eafa5355148b7177ab341b078ab12bb.png) 

In the output of the dir command, the directory files with the < DIR > flag are represented, and the others are normal files. Text files, pictures, audio & video files, etc. are all normal files. View the files in the .idea directory: 

dir .idea 

![avatar]( ba02e599dc143ce29a16aa83ac80fc9f.png) 

(3) type: view file 

Execute the type command to view the contents of the file. The basic syntax of the type command: 

type path_of_file 

path_of_file represents the path to the file and can view the contents of the file across disks. 

Example demonstration: 

Check the hellopython.py in the python3-learning directory of the D disk in the C disk: 

type D:\python3-learning\hellopython.py 

![avatar]( 15dfbb26504fcce1a7a220d5117b6718.png) 

(4) more: view the file 

Executing the more command can also view the contents of the file. The basic syntax of the more command: 

more path_of_file 

path_of_file represents the path of the file, you can view the contents of the file across the disk, compared with the type command, more supports segmented display of the file, when the file is relatively large, it is recommended to use the more command to view. The main options of the more command: 

![avatar]( 45c33496066e6df79d3ae2a28cafe49b.jpeg) 

Example demonstration: 

Check the workspace.xml file in the idea subdirectory under the python3-learning directory of the D disk in the C disk: 

more D:\python3-learning\.idea\workspace.xml 

![avatar]( 4cea17e553c963f72cc6e9038b86568b.png) 

From the output, you can see a prompt for the proportion of content output: 

More (24%) 

It indicates that 24% of the content of the file has been displayed, and pressing the p key of the keyboard will prompt you to enter a number of lines: 

![avatar]( 4067807df2c540cc0ee06e2db809a98e.png) 

Enter the specified number of lines, and the more command will display the next n lines. To exit the display of the More command, press the q key directly on the keyboard. 

(5) mkdir: create directory 

The mkdir command is used to create directories. The basic syntax of the command is: 

mkdir path_of_directory 

Parameter path_of_directory represents the path of the directory, mkdir can collapse the disk to create a directory. 

Create the docs subdirectory under the python3-learning directory of the D disk in the C disk: 

mkdir D:\python3-learning\docs 

![avatar]( 918c9c602a6a02bb886f3ab117937722.png) 

Use the dir command to see if the creation was successful. 

![avatar]( b759473c7a56e4f42b2e373b005a6a35.png) 

From the output of the dir command, it can be seen that the docs directory has been successfully created. The opposite of mkdir is the rd command, which is used to force the deletion of the directory and all files and subdirectories under the directory. When using the rd command to force deletion, you need to add the/s and/q options:, 

![avatar]( 1ac5cf814ca925618c6a2e57bd710f3c.png) 

After executing the rd command to force deletion, the output of the dir command shows that the docs directory has been deleted. 

(6) echo: content output 

Executing the echo command directly will echo the content to the command line: 

![avatar]( 074f8878aa66ed7b8c3edb50b0697553.png) 

With the redirect symbol >, you can write content to a file, and if the file doesn't exist, a new file is created. 

![avatar]( c20f3151cba4e1ba907b74a5bde516db.png) 

The command in the image above is: 

echo > d:\python3-learning\test.py 

It means to write the empty content to the test.py file in the python3-learning directory of the D disk. Since the test.py file does not exist, a new test.py will be created. When executing the dir command to view, you will find that there is an extra test.py file in the python3-learning directory: 

![avatar]( eeb7f915cddee51098290300d9d3c759.png) 

(7) cls: clear screen operation 

Executing the cls command on the command line clears the screen. 

(8) exit: exit the command line 

Executing the exit command on the command line exits the current command line. 

##  4.1.4 Windows environment variables PATH 

(1) Introduction to PATH 

Environment variables are a series of parameters of the operating environment of the system, such as system environment variables PATH. PATH saves parameters related to the path. The system searches for the path saved by PATH in the path search. 

In the command line, you can directly execute the system's built-in commands. If you need to execute third-party installed programs in the command line,

Then the executable program must be added to the environment variables PATH. 

When installing Python in Chapter 1, you can see the options added by PATH on the installation interface: 

![avatar]( 0c675d1e564351339d453423ea349323.png) 

When this option is checked, the system will automatically add the installed Python interpreter to the system environment variables PATH. 

(2) Manually configure PATH 

Add the windows command line and execute the sysdm.cpl command, which will pop up a system property setting window: 

![avatar]( b519eb40f72a7a0ed60d9df1fda0d88a.png) 

Click on the advanced options in the window to see a button for environment variables: 

![avatar]( 361b0bc6933f026400f071100ef7e5f3.png) 

Clicking the environment variables button will bring up the environment variables settings window: 

![avatar]( 194b5a2d3b620de03e5017e8cec3e189.png) 

Among them, the user variable is only valid for the current user, and the system variable is valid for all users in the system. Readers can decide whether to configure user variables or system variables according to the actual situation. When configuring the Path variable, double-click the Path variable with the mouse, and the configuration window of the Path variable will pop up: 

![avatar]( 7515e43d7162f9610768147684e75b10.png) 

Click the New button to add the absolute path of the third-party executable program to the Path variable, and then click OK to complete the configuration process of the Path variable. The same principle applies to the configuration of other environment variables. 

##  4.1.5 system to learn Python 

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning 

