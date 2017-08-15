# Ansible Playbooks and Roles

* Playbooks are expressed in YAML format which tries to be a model of a configuration or a process.
* Each playbook is composed of one or more ‘plays’ in a list.
* By composing a playbook of multiple ‘plays’, it is possible to orchestrate multi-machine deployments, running certain steps on all machines in a server group.
* While it is possible to write a playbook in one very large file, eventually you’ll want to reuse files and start to organize things.
* Roles allow tasks to be packaged together, and can include variables, handlers, or even modules and other plugins.