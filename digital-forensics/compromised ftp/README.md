# Compromised FTP

- **Category:** digital forensics
- **Points:** 25

## Challenge:

> We detected some malicious activity on our FTP server. Someone has performed bruteforce attack to gain access to our FTP server. Find out the Compromised FTP account username & the attacker IP from the following.

## Solution:

We can execute the following command to find the right user and ip.
```
$ cat ftp.log | cut -c 36- | sort -u | grep -v 'FAIL LOGIN'
[ftpuser] OK LOGIN: Client "::ffff:192.168.1.7"
```

**Flag:**`KCTF{ftpuser_192.168.1.7}`

