About
=====

Install docker platform with [Ansible](https://www.ansible.com/).

Ansible is a radically simple IT automation platform that makes your applications and systems easier to deploy.


Requirements
=====

- OS: Ubuntu 14.04 (trusty)
- [Ansible >= 2.0](https://github.com/ansible/ansible)


Usage
=====

Deploy docker without hosts file
```
ansible-playbook -i '192.168.0.1,' playbook.yml
```

Deploy docker with hosts file (Make sure hosts file is you need)
```
ansible-playbook -i hosts playbook.yml
```

Run as other users or use sudo
```
ansible-playbook -i hosts playbook.yml \
-e "ansible_ssh_pass=secret ansible_sudo_pass=secret sudo=yes"
```


Ansible Variables
=====

* docker_group_members: Add users to docker group

