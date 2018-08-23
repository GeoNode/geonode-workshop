## Customize Metadata (4)

**Resource Base Patching**

```bash
mkdir -p my_geonode/templates/base
cp /home/geo/Envs/geonode/src/geonode/geonode/base/templates/base/_resourcebase_info_panel.html my_geonode/templates/base/
vim my_geonode/templates/base/_resourcebase_info_panel.html
```

```python
    ...
    {% if resource.group %}
    <dt>{% trans "Group" %}</dt>
    <dd><a href="/groups/group/{{ resource.group.name }}/activity/">{{ group }}</a> </dd>
    {% endif %}

    <dt>{% trans "DOI" %}</dt>
    <dd>{{ resource.doi }}</dd>

  </dl>
  ...
```