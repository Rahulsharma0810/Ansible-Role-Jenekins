Ansible-Role-Jenekins
=========

Ansible Role to install Jenekins in Ubuntu

ROAD MAP
--------
- Add admin Password
- Add Centos Support
- Add Plugins Support


Requirements
------------

- Java 8

Role Variables
--------------

```
# Jenekins Keys and Repo
jenkins_key_url: http://pkg.jenkins-ci.org/debian/jenkins-ci.org.key
jenkins_repo_url: deb http://pkg.jenkins-ci.org/debian binary/
```

```
# Default is 8080
Port: 5656
```

```
# Installation of Packages
Tools:
  - jenkins
  - git
  - java-common
  - oracle-java8-installer
  - ca-certificates
  - oracle-java8-set-default
```

Example Playbook
----------------

    - hosts: YOUR-HOST-OR-GROUP
      roles:
    	- Ansible-Role-Jenekins


License
-------

MIT

Author - Rahul Sharma
------------------

[Github](https://github.com/Rahulsharma0810)

[Facebook](https://www.facebook.com/rahulsharma0810)