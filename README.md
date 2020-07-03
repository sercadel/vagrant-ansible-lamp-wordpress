# Proyecto Vagrant - Ansible - LAMP - WordPress

---

#### Máquinas

- **Vagrant Ansible**
  - Controlador


- **Vagrant Node**
  - loadbalancer
  - webserver-one
  - webserver-two
  - dbserver

---

#### Ansible

- **loadbalancer**
  - haproxy


- **webserver**
  - apache2
  - php
  - wordpress


- **dbserver**
  - mysql

---

### Ejecutar los playbooks

```console
ansible-playbook -i loadbalancers loadbalancers.yml
ansible-playbook -i webservers webservers.yml
ansible-playbook -i dbservers dbservers.yml
```
