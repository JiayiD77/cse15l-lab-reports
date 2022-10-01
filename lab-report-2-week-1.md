# Lab Report Week 1
* Installing VScode
![Image](https://github.com/JiayiD77/cse15l-lab-reports/blob/main/Week1/VScode.jpg)
Download the VScode from the official website. Get the VScode installed following the instructions.

* Remotely Connecting
![Image](https://github.com/JiayiD77/cse15l-lab-reports/blob/main/Week1/Remotely%20control.png)
Login with *ssh* + *username* at the terminal of the VScode. Password is needed for this process. I changed my password for the 15L specific account but it was not working during the lab session so I used my UCSD account instead. 

* Trying Some Commands
![Image](https://github.com/JiayiD77/cse15l-lab-reports/blob/main/Week1/Commands.png)
![Image](https://github.com/JiayiD77/cse15l-lab-reports/blob/main/Week1/Command2.jpg)
I tried out some commands on the remote computer. Some of them gave results and some of them didn't. It is my first time using these commands, so I defititely need more practice. But it was fun. 
![Image](https://github.com/JiayiD77/cse15l-lab-reports/blob/main/Week1/command3.png)
Command *cd* did not produce any output on the remote computer. However, I can see changes if I used this command on my pc and shown above. 

* Moving Files with scp
![Image](https://github.com/JiayiD77/cse15l-lab-reports/blob/main/Week1/Moving%20files.png)
Moving files was a fun one. The format of the command should be *scp fileName accountName:~/directory*. I forget to add directory path at the first time so this is a pretty important point for me to remember. However, it is kind of tedius to type the password again and again. 

* Setting an SSH Key
![Image](https://github.com/JiayiD77/cse15l-lab-reports/blob/main/Week1/ssh.jpg)
For this step, I need to create a public and private key set on my computer first using *ssh-keygen*. Then using the directory pass and copy the public key onto the remote computer. Then I don't need to type my password to login and copy files.

* Optimizing Remote Running
![Image](https://github.com/JiayiD77/cse15l-lab-reports/blob/main/Week1/optimize.jpg)
With the ssh key set, I can directly include commands while login. As long as I seperate different commands with colon, it will be fine.


