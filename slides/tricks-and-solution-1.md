## Behind the magic

**Hints and tricks**

* *Set the correct OAuth2 server FQDN to GeoServer*

```bash
$ sudo vi /usr/share/geoserver/data/security/filter/geonode-oauth2/config.xml
# edit the configuration of GeoServer security for the oauth2 provider
```
* *Make sure it contains these values:*

```xml
<!-- GeoNode accessTokenUri -->
<accessTokenUri>http://localhost/o/token/</accessTokenUri>
<!-- GeoNode userAuthorizationUri -->
<userAuthorizationUri>http://localhost/o/authorize/</userAuthorizationUri>
<!-- GeoServer Public URL -->
<redirectUri>http://localhost:8001/geoserver</redirectUri>
<!-- GeoNode checkTokenEndpointUrl -->
<checkTokenEndpointUrl>http://localhost/api/o/v4/tokeninfo/</checkTokenEndpointUrl>
<!-- GeoNode logoutUri -->
<logoutUri>http://localhost:8001/account/logout/</logoutUri>
```

