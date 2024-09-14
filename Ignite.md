# SCANNING

I used nmap to run a scan to check for opened ports and i saw just one port opened. 

![image](https://github.com/user-attachments/assets/707a32cf-4884-421c-9289-2bb9e0cd8157)

I did further scanning on this to see if there was anything and yes i got something(it was not really helpful tho)

![image](https://github.com/user-attachments/assets/3154ecc8-7c0f-452a-9332-d76c7b710d81)

# ENUMERATION

I pasted the ip in my browser and it gave me a page, a FUEL CMS page. I tried moving round but there was nothing, Using the image of the second scan with nmap, i still use coconut head to check robots.txr and still nothing too. I did a directory fuzzing
and i got a number of directories.

![image](https://github.com/user-attachments/assets/0231f25d-f270-4bba-8008-48c10cc40bce)

I navigated to the directories but there was nothing also so I checked the ```/fuel``` directory i saw from the nmap scan, it brought a login page and i entered admin admin as login and pass as it was shown there.

![image](https://github.com/user-attachments/assets/44f70a8a-2916-47e0-b6a0-d629e119389e)

Checked round after logging in but nothing still so i decided to check online if there was any exploit on the version of the fuel cms. I used searchsploit for that.

![image](https://github.com/user-attachments/assets/e918cec4-edf4-4e0b-907c-7971a4d19405)

# EXPLOITATION

After finding the exploit, I saved it to it to my machine/

![image](https://github.com/user-attachments/assets/1b3cd828-ad11-4b8a-b6cc-5de3f70285ba)

I ran the first one against the url. 

PS: I changed the name before running it. For some reasons, it kept giving an error which i did not understand so I used the third exploit and it gave a shell. 

![image](https://github.com/user-attachments/assets/fe6e75b2-68e2-41b1-a4fd-148369f17499)

From here i needed to change it to a reverse shell so i can work better on my terminal. I used an online reverse shell generator to get the commands to use as both the listener and the attacker to get a reverse shell
