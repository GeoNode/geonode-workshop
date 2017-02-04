## Install GeoNode into Ubuntu

* The command `sudo apt-get install geonode` may create issues if your system `locale` is not correctly configured.

* In order to fix this, please follow the procedures below. **If everything went well, you can skip those passages**

```bash
$ sudo locale-gen en_US
$ sudo locale-gen en_US.UTF-8
$ sudo locale-gen it_IT.ISO-8859-1
$ sudo locale-gen it_IT.UTF-8
$ sudo locale-gen it_IT.ISO-8859-15@euro
$ sudo update-locale
# Update Locale
```
---

```bash
$ export LC_ALL=en_US.UTF-8
$ export LANG=en_US.UTF-8
$ export LANGUAGE=en_US.UTF-8
$ sudo dpkg-reconfigure geonode
# Export locale env vars and reconfigure geonode
```
---

