LDAP auth settings
====================

**These are the environments that were configured:**

- dev
- qa
- prod
- db
- dbdev

**These are the ldap roles and groups configured:**

- DEVELOPER
- DBA
- DEVOPS
- SRO

Depending on the environment (env) it would configure some groups to have access to the server

**playbook run:**

ansible-playbook -i hosts ldap_auth.yml -e "env=dbdev"
