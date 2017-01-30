## Initialize GeoNode systemwide

```bash
$ geonode createsuperuser
# a commandline toolkit has been installed systemwide so let's create the superuser of the GeoNode instance
# use username: 'geonode' and password: 'geonode'

$ sudo geonode-updateip localhost:8001
# update the address where the GeoNode instance is running
```

**You have installed GeoNode! Congratulations!!!**

Anyway you don't have GeoNode available from your local browser.
So we have to set a new forwarding port in the vagrantfile:

```bash
config.vm.network "forwarded_port", guest: 80, host: 8001
# This port has to be the same of that before and equal between guest and host. You can understand this later on.
# Again don't use a port lower than 1024 on your host machine (not privileged)!!!
```

After this you have to reload the vagrant configuration:

```bash
$ vagrant reload
# reload vagrantfile with the new configuration
```
