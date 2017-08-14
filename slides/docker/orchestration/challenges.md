# Challenges

* GeoNode is a web application in the browser so it is expected to being navigated from the address of the Docker Host machine

* [Docker-machine](http://docker.com) does set the *DOCKER_HOST* variable while Docker native and derivates doesn't

* GeoNode components need to know the address of the front-end site where the user is going to navigate the application for configuring settings and authentication and authorization urls for the **OAuth2** security mechanism

Solutions:

- Container
```bash
docker run --net=host codenvy/che-ip:nightly
```
**Credits to Codenvy/Eclipse Foundation**
