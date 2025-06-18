### **Standard FHS directories**

* **/home**: Each user in the system gets their own home directory.  
* **/bin**: This directory stands for “binary” and contains binary files and other executables.   
* **/etc**: This directory stores the system’s configuration files.  
* **/tmp**: This directory stores many temporary files. The **/tmp** directory is commonly used by attackers because anyone in the system can modify data in these files.  
* **/mnt**: This directory stands for “mount” and stores media, such as USB drives and hard drives.

## **Key commands for navigating the file system**

### **pwd**

The **pwd** command prints the working directory to the screen. 

**ls**

The **ls** command displays the names of the files and directories in the current working directory.

### **cd**

The **cd** command navigates between directories. When you need to change directories, you should use this command.

## 

## 

## **Common commands for reading file content**

### **cat**

The **cat** command displays the content of a file.

### **head**

The **head** command displays just the beginning of a file, by default 10 lines.

### **tail**

The **tail** command does the opposite of **head**. This command can be used to display just the end of a file, by default 10 lines.

### **less**

The **less** command returns the content of a file one page at a time.

# Filter content in Linux

## **grep**

The grep command searches a specified file and returns all lines in the file containing a specified string or text.

## 

## **Piping**

The pipe command is accessed using the pipe character (**|**). Piping sends the standard output of one command as standard input to another command for further processing.

## **find**

The **find** command searches for directories and files that meet specified criteria.

### **\-name and \-iname**

One key criteria analysts might use with **find** is to find file or directory names that contain a specific string.

### **\-mtime**

Security analysts might also use **find** to find files or directories last modified within a certain time frame.

## **Creating and modifying directories**

### **mkdir**

The **mkdir** command creates a new directory.

### **rmdir**

The **rmdir** command removes, or deletes, a directory.

## 

## 

## **Creating and modifying files**

### **touch and rm**

The **touch** command creates a new file.

### **mv and cp**

The **mv** command moves a file or directory to a new location, and the **cp** command copies a file or directory into a new location.

## **nano text editor**

nano is a command-line file editor that is available by default in many Linux distributions.

# Permission commands

* read: for files, this is the ability to read the file contents; for directories, this is the ability to read all contents in the directory including both files and subdirectories  
* write: for files, this is the ability to make modifications on the file contents; for directories, this is the ability to create new files in the directory  
* execute: for files, this is the ability to execute the file if it’s a program; for directories, this is the ability to enter the directory and access its files

These permissions are given to these types of owners:

* user: the owner of the file  
* group: a larger group that the owner is a part of  
* other: all other users on the system

Few important **ls** options for security analysts:

* **ls \-a**: Displays hidden files. Hidden files start with a period (**.**) at the beginning.  
* **ls \-l**: Displays permissions to files and directories. Also displays other additional information, including owner name, group, file size, and the time of last modification.  
* **ls \-la**: Displays permissions to files and directories, including hidden files. This is a combination of the other two options.

### **Using chmod**

The **chmod** command requires two arguments. The first argument indicates how to change permissions, and the second argument indicates the file or directory that you want to change permissions for. 

# Use of sudo command

The **sudo** command is important for security analysts because it allows users to have elevated permissions without risking the system by running commands as the root user.

### **useradd**

The **useradd** command adds a user to the system.

* **\-g**: Sets the user’s default group, also called their primary group  
* **\-G**: Adds the user to additional groups, also called supplemental or secondary groups

### **usermod**

The **usermod** command modifies existing user accounts.

* **\-d**: Changes the user’s home directory.  
* **\-l**: Changes the user’s login name.  
* **\-L**: Locks the account so the user can’t log in.

### **userdel**

The **userdel** command deletes a user from the system.

### **chown**

The **chown** command changes ownership of a file or directory.

