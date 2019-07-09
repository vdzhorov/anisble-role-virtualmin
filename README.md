# ansible-role-virtualmin

Basic Virtualmin installation with Ansible

### Prerequisites

* ansible-role-hostname (Needed in order to set FQDN beforehand. This is required by Virtualmin.)

## Deployment

Example playbook:

```
- hosts: web1
  roles:
    - 'ansible-role-virtualmin'
```

Set your prefered bundle (LAMP or LEMP) in vars/main.yml. After that simply run your playbook:

```
ansible-playbook -i '<TARGET_HOST_IP>,' playbooks/mariadb.yml
```

## Built With

* [Ansible 2.8](https://docs.ansible.com/ansible/2.8/index.html)

## Authors

* **Valentin Dzhorov** - *Initial work* - [vdzhorov](https://github.com/vdzhorov)

## Company

* **Delta.BG**

## License

This project is licensed under the MIT License.
