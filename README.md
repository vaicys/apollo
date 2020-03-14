[Ansible isntall instruction](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

Execute ansible playbook:
```
$ ansible-playbook -i "[hostname]," site.yml --vault-password-file ~/vault_key
```
Encrypt command:
```
$ ansible-vault encrypt --vault-password-file ~/vault_key [filename]
```
Descrypt command:
```
$ ansible-vault encrypt --vault-password-file ~/vault_key [filename]
```
