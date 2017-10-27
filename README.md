Shadowsocks
=========

Ansible role that build the shadowsocks-libev from source.

Role Variables
--------------

Variables you can rewrite:

```
ss_password: '!password'
ss_server_port: 443
ss_local_port: 1080
ss_timeout: 300
ss_method: 'aes-cfb-256'
```


Example Playbook
----------------

Install `waste-time.shadowsocks` role first:

```
$ ansible-galaxy install waste-time.shadowsocks
```

Rewrite `ss_password`, `ss_method` and `ss_server_port`:

    - hosts: servers
      roles:
         - { role: 'waste-time.shadowsocks', ss_password: 'password', ss_method: 'aes-256-cfb', ss_server_port: 8838 }

have fun.

License
-------

BSD

Author Information
------------------

wall2flower (luotao.ruby@gmail.com)

