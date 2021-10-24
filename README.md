# Selectel test task

This repo contains the solution of Selectel test task.

#### Usage:
  - Create python3 virtual environment and activate it
  - Install packages from requirements.txt to your venv via: `$ python -m pip install -r requirements.txt`
  - Run playbook: `$ ansible-playbook -i inventory/prod.ini playbook.yml`

#### Cluster info:
domain-name: `flood-resident.tk`

k8s-master:
  - ip: `31.184.218.184`
  - root_pass: `5iRhXrYIY4ps`
  - user: `ansible`
  - user_pass: `123`

k8s-worker-01-ip: 
  - ip: `91.206.14.193`
  - root_pass: `l9tFBzn9N9oG`
  - user: `ansible`
  - user_pass: `123`
