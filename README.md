ansible-digitalocean-students
=============================

This role creates 3 CentOS 7 vms on digital ocean for each student.

Variables
---------

* digitalocean_token: ```The Digital Ocean access token```
* admin_keys: ```Administrator public ssh keys```
* students: ```The list of students```


Example
-------

```yaml
- name: create student vms
  vars:
    digitalocean_token: XXX
    admin_keys:
      - name: kaik
        key: AAAA...
    students_count: 1
    roles:
      - role: ansible-digitalocean-students
```

Author
------

Kai Kahllund <kai.kahllund@akra.de>