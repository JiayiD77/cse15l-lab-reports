# Lab Report 1
* Installing VScode
![Image](https://user-images.githubusercontent.com/114614626/193378137-4eebfc91-7317-4a10-b0d3-f5e855ca1dcf.jpg)
Download the VScode from the official website. Get the VScode installed following the instructions.

* Remotely Connecting
![Image](https://user-images.githubusercontent.com/114614626/193378152-81d9051a-313b-4d61-8397-75feca39602e.png)
Login with *ssh* + *username* at the terminal of the VScode. Password is needed for this process. I changed my password for the 15L specific account but it was not working during the lab session so I used my UCSD account instead. 

* Trying Some Commands
![Image](https://user-images.githubusercontent.com/114614626/193378162-14e0f492-f9a1-4119-b52d-5794807b617c.png)
![Image](https://user-images.githubusercontent.com/114614626/193378160-69d53467-8e5a-44cf-9938-121ba24aea37.jpg)
I tried out some commands on the remote computer. Some of them gave results and some of them didn't. It is my first time using these commands, so I defititely need more practice. But it was fun. 
![Image](https://user-images.githubusercontent.com/114614626/193378161-071ae91b-a1cd-481b-bb46-d576383745fa.png)
Command *cd* did not produce any output on the remote computer. However, I can see changes if I used this command on my pc and shown above. 

* Moving Files with scp
![Image](https://user-images.githubusercontent.com/114614626/193378170-554a1bb5-6711-4ffa-a1a5-e98a2a964bbb.png)
Moving files was a fun one. The format of the command should be *scp fileName accountName:~/directory*. I forget to add directory path at the first time so this is a pretty important point for me to remember. However, it is kind of tedius to type the password again and again. 

* Setting an SSH Key
![Image](https://user-images.githubusercontent.com/114614626/193378172-9212d4da-1199-43da-9544-1f860e221cde.jpg)
For this step, I need to create a public and private key set on my computer first using *ssh-keygen*. Then using the directory pass and copy the public key onto the remote computer. Then I don't need to type my password to login and copy files.

* Optimizing Remote Running
![Image](https://user-images.githubusercontent.com/114614626/193378171-45dbb17e-ac32-45c4-8f27-a806adb0268b.jpg)
With the ssh key set, I can directly include commands while login. As long as I seperate different commands with colon, it will be fine.


