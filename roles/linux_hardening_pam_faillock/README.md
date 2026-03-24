#### Role for faillock.so
1. Always think about what you are doing with PAM, my configure may not be suitable for your environmen

#### Tested on
1. Debian 13 (trixie)
2. Ubuntu 24.04.4-live-server
3. Rocky Linux 10

#### Note
1. pam_faillock is meant to protect from brute force attacks. It does not mean to protect from configured SSH public key authentication!
2. Why did I choose to configure PAM files directly in Debian? Unfortunately, I encountered some unexpected behavior with the `pam-auth-update` utility, and the “community.general.pamd” module doesn't give me the flexibility I need. I might change my approach in the future.