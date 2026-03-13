#### Ansible test ping!
```shell
ansible localhost -m ping -i inventory -u root --private-key=~/.ssh/u_key -k
```
> use option '-k' if u key have parsphere.

#### Note
1. At the moment I do not use a virtual environment and ssh agent.
2. If u have any comments, corrections or suggestions, please create an issue, don't be shy. (:
3. There will be encryption used in some places - don't worry, you can change that.
