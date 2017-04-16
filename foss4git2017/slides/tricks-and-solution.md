## Behind the magic

**Security hints and tricks**

Security in GeoServer is hugely changed with the introduction of **[OAuth2](http://docs.geonode.org/en/master/tutorials/admin/geoserver_geonode_security/)**

* *Be sure that the ports are available to your host machine*
```bash
config.vm.network "forwarded_port", guest: 80, host: 8001
# config.vm.network "forwarded_port", guest: 8080, host: 8080 # Optional,
# enable if you don't need to reproduce a fully GeoNode proxied use case
# forward another port to the host. You need to 'vagrant reload' to apply the changes
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

