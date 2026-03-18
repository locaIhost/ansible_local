#### Read it
1. To run it, you need to generate a key and change the tgmptp_key variable in host_vars or role, idk  knowing what role organization you are using.
```shell
openssl rand -hex 16
```
2. Make the tgmptp_tag variable empty.
3. Launch the role.
4. You can get the TAG from @MTProxybot, then restart the role with the tgmptp_tag variable set.
---
I'll probably add a pre tasks for key generation later.