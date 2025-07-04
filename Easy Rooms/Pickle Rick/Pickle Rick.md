# Room Info

### Name: Pickle Rick
Description: This Rick and Morty-themed challenge requires you to exploit a web server and find three ingredients to help Rick make his potion and transform himself back into a human from a pickle.

Expected Time: 30 mins

Room Link: https://tryhackme.com/room/picklerick


# Steps to Hack & Notes for Blue Team
1. Scan the port using Nmap, using http-enum NSE script to enumerate directories used by web servers.
```bash
nmap -sV -p 80,443 --script http-enum 10.10.231.214
```
<img src="img/PR1.png" alt="Pickle Rick" width="500"/>
As we can see, there is a login.php page:
<img src="img/PR3.png" alt="Pickle Rick" width="500"/>
and a robots.txt page:
<img src="img/PR4.png" alt="Pickle Rick" width="500"/>

<span style="color:blue;"><i>BT Notes: To limit Nmap enumeration, </i></span>

2. The robots.txt page seems to contain the password. To find the username, we view the page source code with the shortcut Ctrl + U:
4. 

3. 
# Final Reflection
