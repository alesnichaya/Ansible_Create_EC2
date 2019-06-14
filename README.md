# Ansible_Create_EC2
1)Since AWS keys are sensitive data, we must use Ansible Vault.
`ansible-vault create aws_keys.yml`

2)

3) Run playbook
```ansible-playbook task.yml --ask-vault-pass```
