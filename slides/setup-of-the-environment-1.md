## Setup of GeoNode in a box

Start the virtual machine:

- Vagrant needs a VirtualBox installed on your system to start. Download it and install from [VirtualBox](http://docs.geonode.org/en/latest/tutorials/install_and_admin/vm_setup_virtualbox.html).

- With the latest bersions of VirtualBox, you may also need to update your Vagrant system. Downloaf and install the latest version from [Vagrant](https://www.vagrantup.com/downloads.html).

```bash
$ vagrant up --provider=virtualbox
# Start the virtual machine as defined into the vagrantfile
```

Login with a bash shell into the box

```bash
$ vagrant ssh
# Get into the box with the vagrant user
```
