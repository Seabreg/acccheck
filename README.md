# acccheck
When you need to access a running Windows system, you can use a dictionary attack tool like acccheck to brute-force the admin's username and password as long as it's older Windows system (XP and earlier, possibly Windows 7).

Acccheck looks at Windows SMB protocol authentication, specifically the administrator account, and works over the network. Of course, if you have physical access to your machine, there are other ways to get the password, but if not, acccheck is a good tool. And best of all, it's built right into Kali.

# Usage
acccheck -t 10.0.2.15 -U /usr/share/dirb/wordlists/others/names.txt -P /usr/share/dirb/wordlists/big.txt
