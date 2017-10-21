Shadowsocks
=========

Ansible role that build the shadowsocks-libev from source.

Role Variables
--------------

Variables you can rewrite:

```
ss_password: '!password'
ss_server_port: 8389
ss_local_port: 1080
ss_timeout: 300
ss_method: 'chacha20'
```


Example Playbook
----------------

Rewrite `ss_password`, `ss_method` and `ss_server_port`:

    - hosts: servers
      roles:
         - { role: 'wall2flower.shadowsocks', ss_password: 'password', ss_method: 'aes-256-cfb', ss_server_port: 23333 }

License
-------

BSD

Author Information
------------------

wall2flower (luotao.ruby@gmail.com)

