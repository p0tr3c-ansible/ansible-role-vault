# Ansible Role: Vault

Install Hshicorp vault on Centos7

## Requirements

None

## Role Variables

All role variables are listed in default/main.yml.

## Dependencies

None.

## Example Playbook

    - hosts: vault
      become: yes
      tasks:
        - name: Install vault
          include_role:
            name: ansible-role-vault
          vars:
            aws_bucket_name: bucket
            aws_region: eu-west-1
            vault_tls_enabled: False


## License

MIT / BSD
