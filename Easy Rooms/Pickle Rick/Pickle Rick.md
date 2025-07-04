# Room Info

### Name: Pickle Rick
Description: This Rick and Morty-themed challenge requires you to exploit a web server and find three ingredients to help Rick make his potion and transform himself back into a human from a pickle.

Expected Time: 30 mins

Room Link: https://tryhackme.com/room/picklerick


# Steps to Hack & Notes for Blue Team
1. Looking the IP adress will direct us to this site
   
2. Scan the port using Nmap, using http-enum NSE script to enumerate directories used by web servers.
```bash
nmap -sV -p 80,443 --script http-enum 10.10.231.214
```
4. 

3. 
# Final Reflection
