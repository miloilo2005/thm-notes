# TryHackMe Notes
Notes for TryHackMe things

## Recon Phase
- Use Nmap:
```bash
nmap -sC -sV -T4 -p- <target_ip>
```
Once we know the open ports, we use this for web:
```bash
nmap -p 80,443 --script=http-title,http-enum,http-methods <target_ip>
```
We use this for SMB:
```bash
nmap -p 139,445 --script=smb-enum-shares,smb-enum-users <target_ip>
```
