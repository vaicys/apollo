Continuous deployment with Travis CI  
[![Travis CI build](https://travis-ci.org/vaicys/apollo.svg?branch=master)](https://travis-ci.org/vaicys/apollo)

To install the latest Ansible version, follow the [official](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) instructions.

To execute the playbook:
```
# do not skip the comma at the end of the fully qualified domain name
$ ansible-playbook -i "[FQDN]," [--vault-password-file VAULT_KEY] [--private-key PRIVATE_KEY_FILE] [-u REMOTE_USER] site.yml
```

To work with encrypted variable files:
```
$ ansible-vault encrypt --vault-password-file ~/vault_key [filename]

$ ansible-vault decrypt --vault-password-file ~/vault_key [filename]
```
