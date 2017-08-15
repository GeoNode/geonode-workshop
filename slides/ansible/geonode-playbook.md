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