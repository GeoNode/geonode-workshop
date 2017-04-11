## Behind the magic

**Hints and tricks**

*Check the settings of GeoServer Global Proxy Base and Default Authentication Provider*

```bash
$ sudo vi /usr/share/geoserver/data/security/auth/geonodeAuthProvider/config.xml
# edit configuration of default GeoServer authentication provider
$ sudo vi /usr/share/geoserver/data/global.xml
# edit configuration of default GeoServer proxy base url
```

Change with these values:

```xml
<baseUrl>http://localhost:8001/</baseUrl>
<!-- base url of geonode web server -->
```

Leave the default for this vagrant configuration:

```xml
<proxyBaseUrl>http://localhost:8080/geoserver</proxyBaseUrl>
<!-- proxy base url of geonode web server - -->
```

Restart the server:

```bash
$ sudo service tomcat7 restart
# restart Tomcat
```
