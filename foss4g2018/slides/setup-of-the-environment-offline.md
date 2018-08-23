## Setup of GeoNode in a box

Installation of minimal requirements from [GeoNode tutorials](http://docs.geonode.org/en/master/tutorials/index.html):

- Download and install latest version of [VirtualBox](http://docs.geonode.org/en/latest/tutorials/install_and_admin/vm_setup_virtualbox.html)

- Download and install [Vagrant](http://docs.geonode.org/en/latest/tutorials/install_and_admin/vm_running_vagrant.html)

- Setup of a VM with a Vagrantfile assuming you are on unix **starting from a provided Vagrant BOX**:

```bash
$ mkdir geonode && cd geonode
$ vagrant box add geonode-ws.box --name ubuntu/geonode-ws
$ vagrant init ubuntu/geonode-ws
```

- Edit the *vagrantfile* for more memory (see issue [#2076](https://github.com/GeoNode/geonode/issues/2076)):

```bash
config.ssh.username = "ubuntu"
config.ssh.password = "ubuntu"
config.vm.provider "virtualbox" do |vb|
    vb.memory = "6144"
end
```

