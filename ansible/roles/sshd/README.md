# sshd

Configure sshd.

## Role variables

- `sshd_password_authentication`: Optional bool. Whether to enable password login. Default `false`.
- `sshd_disable_forwarding`: Optional bool. Whether to disable all forwarding features (X11, ssh-agent, TCP and StreamLocal). Default `true`.
- `sshd_conf_src`: Optional string. Path to sshd configuration template. Default is in-role template.
- `sshd_conf_dest`: Optional string. Path to destination for sshd configuration file. Default is `/etc/ssh/sshd_config.d/10-ansible.conf` which overrides `50-{cloud-init,redhat}` files, if present.
