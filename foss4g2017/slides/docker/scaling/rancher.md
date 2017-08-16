# Scaling GeoNode with Rancher

To run services into Rancher with a scale put a `rancher-compose.yml` in the same directory of the Docker Compose file:

```
version: '2'
services:
  # Reference the service that you want to extend
  geonode:
    scale: 2
```

then run

```
rancher compose up
```

[]()
