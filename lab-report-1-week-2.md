# Guide to Remote Access for CSE15L Students
## **Installing VScode**
Downloading VScode is as easy as visiting this [download link](https://code.visualstudio.com/download)! 
The link should bring you to a site that looks like the image below.

![image](./vscDownload.png)


Click the download button for your respective software to start the download and follow the steps to download VScode on your machine.

## **Remotely Connecting**

### 1. Getting started with SSH

SSH is a program that allows us to access computers remotely from your own machine. MacOS automatically has SSH, so if you are on a Mac you can skip this step. 

However, for Windows, you can use this 
[link](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse) 
and follow the steps to get started with your download. 

### 2. SSH in VScode

In order to access SSH from VScode, open a new terminal. You can do this by using the ` key or by using 
Terminal &rarr; New Terminal in the dropdown menu options.

In the terminal, use the command <br>
`$ ssh cs15lsp22zz@ieng6.ucsd.edu` (but with your credentials) <br> in order to sign onto a computer remotely. 

If it is your first time logging onto a machine remotely, you may get a message stating <br> `Are you sure you want to continue connecting (yes/no/[fingerprint])?` <br>
Make sure to respond yes to these messages.

After logging in, you should see something like this:
![image](./login.png)

## **Trying Some Commands**

### Great! Now that you've successfully connected to your remote machine, let's try playing with it. 

Some commands include `cd`, `ls`, `pwd`, `mkdir`, and `cp`. 

## **Moving Files with `scp`**

## **Setting an SSH Key**

## **Optimizing Remote Running**