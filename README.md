GNS3
=========

Installs and configure GNS3 for the user.

Requirements
------------

The following collections are required:

- community.general

They can be installed by running `ansible-galaxy collection install $COLLECTION`.

To include this role in your `requirements.yml` file, add the following list item:

```yaml
---
roles:
  - name: whalej84.gns3
    src: https://github.com/WhaleJ84/ansible-role-gns3.git
    scm: git

collections:
  - community.general
```

Example Playbook
----------------

This example playbook shows how I would use this role, with custom variables to suit my needs.

```yaml
---
- hosts: localhost

  roles:
    role: whalej84.gns3
    tags: [ gns3 ]
```
