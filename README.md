Ansible-Role-Jenekins
=========

Ansible Role to install Jenekins in Ubuntu

ROAD MAP
--------
- ~~Add admin Password~~
- Add Centos Support
- Add Plugins Support


Requirements
------------

- Java 8 - [Ansible-Role-JRE](https://github.com/Rahulsharma0810/Ansible-Role-JRE)

Role Variables
--------------

```
# Jenekins Keys and Repo
jenkins_deb_key_url: https://pkg.jenkins.io/debian-stable/jenkins.io.key
jenkins_deb_repo_url: deb https://pkg.jenkins.io/debian-stable binary/
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
```

Example Playbook
----------------

    - hosts: YOUR-HOST-OR-GROUP
      roles:
    	- Ansible-Role-Jenekins


Credentials
-----------
- Default Auto Genrated Password is in ```/var/lib/jenkins/secrets/initialAdminPassword```
- Console will print this out, you may copy paste
- Head to youhost:5656, Install Plugins and set it up.

License
-------

MIT

Author - Rahul Sharma
------------------

[Github](https://github.com/Rahulsharma0810)

[Facebook](https://www.facebook.com/rahulsharma0810)