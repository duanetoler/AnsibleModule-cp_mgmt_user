# Ansible modules for Check Point Management API set-user and show-user

Copy these modules to your Ansible collection: ~/.ansible/collections/ansible_collections/check_point/mgmt/plugins/modules/

## Module usage:

Get all locally defined users:
```
* cp_mgmt_user_facts:
```

Get a single user:
```
* cp_mgmt_user_facts:
    name: user1
```

Add a user:
```
* cp_mgmt_user:
    name: new_user
    authentication_method: check point password
    password: NewPasswordString
    ignore_errors: true
```

Delete a user:
```
* cp_mgmt_user:
    name: a_user
    state: absent
```

cp_mgmt_user parameters:
```
- name
- color
- comments
- tags
- groups
- authentication_method
- password
- email
- details_level
- ignore_errors
- ignore_warnings
```



