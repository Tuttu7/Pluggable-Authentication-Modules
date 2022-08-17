#### PAM ( Pluggable Authentication Modules )

#### In earlier systems the applications has to check for the /etc/shadow & /etc/passwd for the authentication purspose for users which was very tidious task for system admins so PAM was introduced so that authentication part will be done by the PAM. For example : Helping SSH service for authentication of users. All the application have it's own pam files inside /etc/pam.d/


#### PAM configuration files

```
/etc/pam.d
/etc/security
/var/log/secure
```

#### PAM modules 

```
For 32 bit machine - /lib/security
For 64 bit machine - /lib64/security
```


#### Examples :

```
pam_tally2 - If there are too many failed login for a user account this module will help to lock the user account
pam_unix   - Checking User credentials against /etc/shadow file
pam_localuser - Checking if the user is listed in /etc/passwd file
```




