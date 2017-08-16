# How to scale with Docker

## Docker Compose

Set the number of containers to run for a service:

```
docker-compose scale geonode=2 worker=3
```
---
```
docker-compose scale geoserver=2 worker=3
```
**We are not ready for this latter. See next slide for the challenge**

## Rancher

- [Rancher]() is an open source project that provides a complete platform for operating Docker in production at large scale
- It integrates native Docker management capabilities such as *Docker Machine* and *Docker Swarm*
- Rancher run itself as a set of Docker containers
- It is recommended to review [supported docker version] (http://rancher.com/docs/rancher/v1.6/en/hosts/#supported-docker-versions)
