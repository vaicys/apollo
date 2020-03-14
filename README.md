To install the latest Ansible version, follow the [official](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) instructions.

To execute the playbook:
```
# DO NOT SKIP THE COMMA at the end of the domain name

$ ansible-playbook -i "[fully_qualified_domain_name]," --vault-password-file ~/vault_key site.yml
```

To work with encrypted variable files:
```
$ ansible-vault encrypt --vault-password-file ~/vault_key [filename]

$ ansible-vault decrypt --vault-password-file ~/vault_key [filename]
```
