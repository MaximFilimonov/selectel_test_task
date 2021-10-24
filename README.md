# Selectel test task

This repo contains the solution of Selectel test task.

#### Usage:
Github runner builds helm package and deploys the app to prod environment on each commit, pull_request to master, or if triggered manually.

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
