#### Role for hardening password policy
1. Ideally, use a template for common-password

#### Tested on
1. Debian 13 (trixie)

#### Command for generate (more or less stable, but sometimes there are mismatches with politics)
```shell
pwgen -s1 -n -c -y 16
```