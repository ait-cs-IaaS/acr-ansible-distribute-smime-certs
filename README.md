# Ansible-Role: acr-ansible-distribute-smime-certs

AIT-CyberRange: Distributes previously generated smime certs. 


## Requirements

- Debian or Ubuntu 

## Role Variables

```yaml
# root path of the site cert files
cert_src_path: ""
```

## Example Playbook

```yaml
- hosts: all
  roles:
    - acr-ansible-distribute-smime-certs
      vars:
        cert_main_inbox:
          username: "csirt1"
          email: "csirt1@company.com"
        cert_additional_inboxes: []
```

## License

GPL-3.0

## Author

- Lenhard Reuter