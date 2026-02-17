## Simple how to use

1. Install ansible-core package

```
sudo apt install ansible-core
```

2. Set version variabels in group_vars/all.yaml


3. Make sure target kubernetes host is reachable

```
ansible all -i inventory.ini -m ping
```

4. Deploy kubernetes cluster

Dry run

```
ansible-playbook -i inventory.ini playbook.yaml --check
```

Deploy the kubernetes

```
ansible-playbook -i inventory.ini playbook.yaml
```