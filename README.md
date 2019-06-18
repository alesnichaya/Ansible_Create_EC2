# Ansible_Create_EC2
1) Since AWS keys are sensitive data, we must use Ansible Vault.
`ansible-vault create aws_keys.yml`
past in file aws_access_key:, aws_secret_key: in format described in aws_keys_default
2) Run playbook
`ansible-playbook task.yml --ask-vault-pass`
3) To create an instance, use the tag "create"
`ansible-playbook task.yml --ask-vault-pass --tags "create"`

To install Apache , use the tag "configure"
`ansible-playbook task.yml --ask-vault-pass --tags "configure"`

To terminate instance , use the tag "terminate"
`ansible-playbook task.yml --ask-vault-pass --tags "terminate"`

