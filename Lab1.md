# Lab Report 1

## 1. Visual Studio Code

- First, go to the Visual Studio Code [website](https://code.visualstudio.com/) to download and install the Visual Studio Code on your computer. 
- Remember: Downloading correct version for your operating system is important!
- Once the Visual Studio Code is installed successfully, it should be look like this when you open it:

![Image](Screen Shot 2023-01-12 at 22.03.45.png)


## 2. Remotely Connecting

- First, using the [Link](https://sdacs.ucsd.edu/~icc/index.php) to look up your course-specific account for CSE 15.
- Here is the [tutorial](https://docs.google.com/document/d/1hs7CyQeh-MdUfM9uv99i8tqfneos6Y8bDU0uhn1wqho/edit) that helps you reset your password for the course-specific account.
- Remember: It may take a few miniutes for the account and password to update and work!
- Then, in the environment of Windows system, install Git from the [website](https://gitforwindows.org/).
- After successfully installation, following the steps in this [post](https://gitforwindows.org/) to use git bash in Visual Studio Code.
- Now, open the terminal in VScode(Ctrl or Command + `, or use the Terminal → New Terminal menu option). 
- Type the following in the terminal, but replace ```zz``` by the letters in your course-specific account.
 
  ```$ ssh cs15lwi23zz@ieng6.ucsd.edu``` 
  
- Remember: It should be one, five, l - the lower case of L! And you do not need to type ```$``` in!
- After that, you might see the following message, 

```
⤇ ssh cs15lwi23zz@ieng6.ucsd.edu 
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?
```
NO WORRIES! Since it might be your first time to connect to this server. 
- What you need to do next is just type ```yes``` and press enter.
- After that, once you see ```Password:``` show up, then type the password of your course-specific account in the terminal. 
- If you're successfully logged in, you should see see something like this: 

![Image](Screen Shot 2023-01-14 at 21.45.32.png)

## 3. Trying Some Commands

- Now, let's try run some different commands on the remote computer using the terminal in VScode.
- Here are some examples that you can try: 

1. ```pwd```
2. ```ls```
3. ```ls -lat```
4. ```ls -a```
5. ```cat /home/linux/ieng6/cs15lwi23/public/hello.txt``` 

Here is the example of what these commands should be look like:

![Image](Screen Shot 2023-01-14 at 22.00.17.png)

- Finally, if you want to log out of your remote connecting in your terminal, try using these:
1. press Ctrl-D
2. type ```exit```
