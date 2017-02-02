## Install GeoNode into Ubuntu

From the [**GeoNode** documentation](http://docs.geonode.org/en/master/tutorials/install_and_admin/quick_install.html#linux)

```bash
$ sudo add-apt-repository ppa:geonode/testing #only for workshop
# vagrant is already into sudoers
```
---

```bash
$ sudo apt-get update
# update packages
```
---

```bash
$ sudo apt-get install geonode
# download of all required dependencies for installing GeoNode
```
---

* The command 'sudo apt-get install geonode' may create issues if your system "locale" is not correctly configured. Please see next slide for details.
