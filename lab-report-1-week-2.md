# Installing VScode

After downloading the Visual Studio Code
[Link](https://code.visualstudio.com/)
open a new java file and write the following command. 

In the terminal, use cd to change the directory to your file and input  `javac yourfilename.java` and then `java yourfilename` to run the file.
![Image](downloadvs.png)
&nbsp;  
&nbsp;  
# Remotely Connecting

Find your username on the UCSD website, 
enter `ssh username@ieng6.ucsd.edu` in terminal and you should be asked for password. 

After entering password, you should see the following result. 
![Image](rc.png)
&nbsp;  
&nbsp;  
# Trying Some Commands

Try running the commands 
* cd
* ls
* pwd
* mkdir
* cp 
see what comes up. 
![Image](command.png)
&nbsp;  
&nbsp;  
# Moving Files with scp

Remember the file you created in step one, use `scp yourfilename.java username@ieng6.ucsd.edu:~/` to copy your file.  

you should see the following result in terminal
![Image](scp.png)


And then login in to ssh and use `ls`, you should see your file!!
![Image](sasssd.png)

&nbsp;  
&nbsp;  
# Setting an SSH Key

Enter following command one by one

Here is what you should enter in terminal

```
$ ssh-keygen  

Generating public/private rsa key pair.  

Enter file in which to save the key (/Users/<user-name>/.ssh/id_rsa): /Users/<user-name>/.ssh/id_rsa
Enter passphrase (empty for no passphrase): 
```
you do not need to enter any passphrases.

```
Enter same passphrase again: 
Your identification has been saved in /Users/<user-name>/.ssh/id_rsa.
Your public key has been saved in /Users/<user-name>/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:jZaZH6fI8E2I1D35hnvGeBePQ4ELOf2Ge+G0XknoXp0 <user-name>@<system>.local
The key's randomart image is:
+---[RSA 3072]----+
|                 |
|       . . + .   |
|      . . B o .  |
|     . . B * +.. |
|      o S = *.B. |
|       = = O.*.*+|
|        + * *.BE+|
|           +.+.o |
|             ..  |
+----[SHA256]-----+
```

If you are on windows you need to follow these [extra steps](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement#user-key-generation).

now copy the key to your ssh directory with the following method

```
$ ssh cs15lsp22zz@ieng6.ucsd.edu
<Enter Password>
# now on server
$ mkdir .ssh
$ <logout>
# back on client
$ scp /Users/<user-name>/.ssh/id_rsa.pub cs15lsp22zz@ieng6.ucsd.edu:~/.ssh/authorized_keys
# You use your username and the path you saw in the command above
```
Then you can login without password.
![Image](sd.png)
&nbsp;  
&nbsp; 
# Optimizing Remote Running

run `ls` on the remote server to see the file.

on the server, use command
* `javac yourfilename.java`
* `java yourfilename` to run remotely.
![Image](ls.png)








