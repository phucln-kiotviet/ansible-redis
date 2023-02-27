# Ansible redis

- This is my very first try on ansible, and I choose test with redis :D


- Run ansible with user which difference on local PC:

```sh
ansible-playbook playbooks/playbook.yml --user user --extra-vars "ansible_sudo_pass=12345678"

# or in this repo:
ansible-playbook -vvv -i inventory.yml first-playbook.yml --user ubuntu --extra-vars "ansible_sudo_pass=12345678"
```

- Install redis:

```sh
ansible-playbook -vvv -i inventory.yml playbook-redis.yml --user ubuntu --extra-vars "ansible_sudo_pass=12345678"
```

## Test role
- Create role for demo purpose