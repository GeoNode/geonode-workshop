## Behind the magic

**Hints and tricks**

* *Set the correct OAuth2 Keys to GeoServer*

```bash
$ sudo vi /usr/share/geoserver/data/security/filter/geonode-oauth2/config.xml
# edit the configuration of GeoServer security for the oauth2 provider
```
* *Make sure the clientId and clientSecret keys are the same of the GeoNode ones:*

```xml
<!-- GeoNode OAuth2 Client ID -->
<cliendId>the_geonode_oauth_client_id</cliendId>
<!-- GeoNode OAuth2 Client Secret -->
<clientSecret>the_geonode_oauth_client_secret</clientSecret>
```

