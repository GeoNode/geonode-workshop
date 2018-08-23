## Users and groups

- Registration for new user is disabled by default.
If you want allow users to register autonomously, edit the settings file for enabling that:

```bash
$ sudo vi /etc/geonode/local_settings.py
# systemwide local settings for geonode
```

Change these lines:

```python
REGISTRATION_OPEN = True
ACCOUNT_APPROVAL_REQUIRED = False
ACCOUNT_EMAIL_CONFIRMATION_EMAIL = False
ACCOUNT_EMAIL_CONFIRMATION_REQUIRED = False
# settings related to users registration
```

- Let's get started to create a new user, you can do that because you are an administrator
    - New accounts don't need to be approved
    - You won't be receiving an email to confirm the registration
- A new user can create his/her own groups and will be the manager
