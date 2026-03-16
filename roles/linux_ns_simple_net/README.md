#### NOTE
1. Very experimental
2. I don't like using ansible.builtin.command, but alas. I haven't found a decent way to do this natively using nmcli yet. :(
3. Tested on rhel based deb based
4. Since this kind of thing can currently only be done with iproute or custom modules, i'll leave the nmcli-specific sections commented out. (files: tasks/main.yml, configure_int_veth_to_nss.yml and template/nmconnection)