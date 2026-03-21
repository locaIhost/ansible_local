#### Role for hardening password policy
1. Ideally, use a template for common-password

#### Tested on
1. Debian 13 (trixie)
2. Rocky Linux 10

#### Command for generate (more or less stable, but sometimes there are mismatches with politics)
```shell
pwgen -s1 -n -c -y 16
```
#### Note
1. Why did I choose to configure PAM files directly in Debian? Unfortunately, I encountered some unexpected behavior with the `pam-auth-update` utility, and the “community.general.pamd” module doesn't give me the flexibility I need. I might change my approach in the future.