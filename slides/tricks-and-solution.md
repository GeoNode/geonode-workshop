## Don't panic!

**Security hints and tricks**

Security in GeoServer is hugely changed with the introduction of **[OAuth2](http://docs.geonode.org/en/master/tutorials/admin/geoserver_geonode_security/)**

* *Be sure that the ports are available to your host machine*
```bash
config.vm.network "forwarded_port", guest: 80, host: 8001
config.vm.network "forwarded_port", guest: 8080, host: 8080
# forward to the host another port. You need to 'vagrant reload' to apply the changes
```
* *Double check that the correct GeoNode Base Url has been configure on GeoServer*
```bash
$ sudo vi /usr/share/geoserver/data/security/role/geonode\ REST\ role\ service/config.xml
# edit the configuration of geonode REST role service
```
* *Must contain the following value:*
```xml
<baseUrl>http://localhost:80/</baseUrl>
<!-- base url of geonode web server -->
```

