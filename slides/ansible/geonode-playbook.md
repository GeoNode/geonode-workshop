# GeoNode Playbook

```YAML
- hosts: webservers
    remote_user: ubuntu
    vars:
        app_name: my_geonode
        github_user: GeoNode
        server_name: demo.geonode.org
    roles:
        - { role: GeoNode.geonode }
```

To install with the above `playbook.yml`:

```bash
$ ansible-playbook playbook.yml --ask-sudo-pass
```