# test-openldap Helm Chart

Helm Chart to run an OpenLDAP server prepopulated with test data.

This deploy the [`rroemhild/test-openldap` Docker image](https://hub.docker.com/r/rroemhild/test-openldap) (source: https://github.com/rroemhild/docker-test-openldap).

## Installation
```
git clone https://github.com/manics/helm-test-openldap
helm upgrade --install ldap ./helm-test-openldap --wait
```
An OpenLDAP server will be running inside the cluster on ports 389 (ldap) and 686 (ldaps).
The service can be accessed at `ldap-test-openldap.<namespace>.svc.cluster.local`.

## LDAP users and groups

See the [documentation for `rroemhild/test-openldap`](https://github.com/rroemhild/docker-test-openldap).
