#### Role for changing password expiration date
1. Change [PASS_MAX_DAYS, PASS_MIN_DAYS and PASS_WARN_AGE]
2. Disabling gecos changes
3. Disabled to prevent conflicts with pam_faillock and avoid legacy logging duplication

#### Tested on
1. Debian 13 (trixie)
2. Ubuntu 24.04.4-live-server

#### Note
1. We understand, of course, that in many modern distributions the role of the login.defs file has narrowed? Or use `pam_umask.so`
2. The `PASS_MAX_DAYS` etc. settings do not apply to root and existing users automatically
3. If u not have central auth, bad, why not) ` chage -d 0 $USER` =) self f***
4. If u have enable account inactive see `/etc/default/useradd:INACTIVE`