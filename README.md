GitHub
=========

An Ansible role that bundles the modules from community.general

Requirements
------------

There are a couple of requirements that need to be met in order to use this role.

1. Install the required modules

    ```bash
    ansible-galaxy \
        collection \
        install \
        --requirements-file roles/requirements.yml
    ```

1. Set your required `github_config` and `github_secret` variables as described in `defaults/main.yml` and `defaults/vault.yml`.

1. Install the following `pip` packages and ensure they are available in the Python PATH for the Ansible user.

    ```bash
    pip install \
        --user \
        github3.py \
        PyGithub
    ```

Role Variables
--------------

Descriptions of available variables are commented in `defaults/main.yml`

Dependencies
------------

No dependant roles.

Example Playbook
----------------

```yaml
```

License
-------

Apache 2.0
