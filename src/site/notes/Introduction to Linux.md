---
{"dg-publish":true,"permalink":"/introduction-to-linux/"}
---

## Basic use
 
if we type only cd, [[leads us\|leads us]] to directory of your user, which is hosted in /home
and if we type echo $HOME this show the directory of the current user the same way 
we can see in the left the users and the personal directory we can see [[almost\|almost]] at the end.
and at the end show te shell that we using 
![[Screenshot 2024-01-14 101019.png \|Screenshot 2024-01-14 101019.png ]]
![Pasted image 20240114101409.png](/img/user/Pasted%20image%2020240114101409.png)
In other way if you type echo $SHELL we can see the type of shell that we using 
if we type cat /etc/shells we can see all types of shell and we can change the shell writing the name of the shell for example: bash 
and we can return to the last shell writing exit 
![Pasted image 20240114101756.png](/img/user/Pasted%20image%2020240114101756.png)

---
---

## Flow control stder-stdout, operators and background process 

we can concatenate commands in one liner and also separate them, for example if we writhe 
*whoami; ls* it show our user and also the content of the current directory --------------------
we can write [[as many commands as you want\|as many commands as you want]]. if you type && the same way show the current user and list the content, but the difference is  && causes the second command to be executed only if the first was successful-----------------------------------------------------
If you want to see the status code of te las command, you can write $?---------------------
Also if write || between commands the second also will execute regardless of whether the first was successful 

![Pasted image 20240114103810.png](/img/user/Pasted%20image%2020240114103810.png)![Pasted image 20240114104042.png](/img/user/Pasted%20image%2020240114104042.png)
											we  can redirect an error to /dev/null [[in the following way\|in the following way]]  whoam 2> /dev/null any thing that we redirect here will disappear, it's like a black hole  we can add 2&>1  [[it will become\|it will become]] in stdout, it will take the error as the output of the command and redirect it to /dev/null

 
