# Selectel test task
![](https://github.com/MaximFilimonov/selectel_test_task/actions/workflows/ci-cd.yml/badge.svg)

This repo contains the solution of Selectel test task.

#### Usage:
Github runner builds helm package and deploys the app and k8s infrastructure to prod environment on each commit/pull_request to master, or if triggered manually.

#### Cluster info:
domain-name: `flood-resident.tk`

k8s-master:
  - ip: `31.184.218.184`
  - root_pass: `5iRhXrYIY4ps`
  - user: `ansible`
  - user_pass: `123`

k8s-worker-01: 
  - ip: `91.206.14.193`
  - root_pass: `l9tFBzn9N9oG`
  - user: `ansible`
  - user_pass: `123`


#### Tests:
- Basic Usage:
```
curl -k -X PUT -H "Arbitrary:Header" -d aaa=bbb http://flood-resident.tk/hello-world
```

- Decode JWT header:
```
curl -k -H "Authentication: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c" http://flood-resident.tk/
```

- JSON payloads and JSON output
```
curl -X POST -H "Content-Type: application/json" -d '{"a":"b"}' http://flood-resident.tk/
```

- Add a delay before response
```
curl -v -H "x-set-response-delay-ms: 6000" http://flood-resident.tk/
```
