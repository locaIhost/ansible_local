#### Ansible test ping!
```shell
ansible localhost -m ping -i inventory -u root --private-key=~/.ssh/u_key -k
```
> use option '-k' if u key have parsphere.

#### Example run roles (enable ip_frw)
```shell
ansible-playbook side.yml -i inventory -u root --private-key=~/.ssh/u_key -k -l uap
```
> side.yml is a run file used to more include roles for specific targets
> (use option '-l' for further limit selected hosts).

#### Example run roles and ansible-encrypt
```shell
ansible-playbook side.yml -i inventory -u root --private-key=~/.ssh/u_key -k -l uap --ask-vault-password
```

#### Note
1. At the moment I do not use a virtual environment and ssh agent.
2. If u have any comments, corrections or suggestions, please create an issue, don't be shy. (:
3. There will be encryption used in some places - don't worry, you can change that.
