# aix
```
lsuser <userid>  # check user info: locked status, unsuccessful_login_count, etc
lsuser -a unsuccessful_login_count <userid>   # list unsuccessful_login_count
chsec -f /etc/security/lastlog -a unsuccessful_login_count=0 -s <userid>     # reset unsuccessful_login_count
chuser account_locked=false <userid>  # unlock 
chuser account_locked=true <userid>  # lock 
```
