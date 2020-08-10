Generate SSH key pair
```
ssh-keygen -t rsa -b 2048 -f rsa_key_name
```

Remove host from known_hosts
```
ssh-keygen -R host
```

Get SSH server key fingerprint
```
ssh-keyscan host -> temp_public_key_file
ssh-keygen -l -f temp_public_key_file
```

Detail Documentation: 

   [ssh-keygen](http://man.openbsd.org/cgi-bin/man.cgi/OpenBSD-current/man1/ssh-keygen.1?query=ssh-keygen&sec=1)
   
   [ssh-keyscan](https://man.openbsd.org/ssh-keyscan.1)