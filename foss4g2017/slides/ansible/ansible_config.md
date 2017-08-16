# Ansible Configuration

Ansible keeps track of all of the servers that it knows about through a "hosts" file.

```bash
$ sudo vim /etc/ansible/hosts
```

Example hosts file:
```
[dbservers]
db01.intranet.mydomain.net
db02.intranet.mydomain.net
10.25.1.56
10.25.1.57
```