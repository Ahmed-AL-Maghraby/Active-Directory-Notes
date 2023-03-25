# Active-Directory-Notes
Active Directory Notes

<br>

# Enumeration

=> Port 139/445 to enumerate the NetBIOS for information such as the existing usernames, NetBIOS-Domain Name, SID, etc

```
$ enum4linux <ip>
```

 => Enumerating Users via Kerberos
 
```
$ wget https://github.com/ropnop/kerbrute/releases/download/v1.0.3/kerbrute_linux_amd64
$ chmod +x kerbrute_linux_amd64

# user list and password list

$ wget https://raw.githubusercontent.com/Sq00ky/attacktive-directory-tools/master/userlist.txt
$ wget https://raw.githubusercontent.com/Sq00ky/attacktive-directory-tools/master/passwordlist.txt

$ ./kerbrute_linux_amd64 userenum --dc=<ip> -d=<domain>.  userlist.txt

```


#  Exploitation Abusing Kerberos








 
