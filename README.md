# Description
Simple playbook and vagrant files to test an installation of logstash on a specific linux distribution

# Warning
- The ansible playbook should not be used on a production setup
- If you want real provisioning see the official https://github.com/elasticsearch/puppet-logstash

# Requirements
- [Vagrant](http://vagrantup.com)
- [Ansible](http://ansibleworks.com)
- [Virtualbox](http://virtualbox.org)

# How to run?
- puts the logstash packages in the packages directory
- create a symlink current.deb or current.rpm
- cd distribution/
- vagrant up
- You can test uninstall and upgrade using env variable like `STEP=uninstall,upgrade vagrant up`

# Defaults
- It will install the required jvm
- It will create a sample testing.conf (this config use the generator to create a file in /tmp/testing.log)
- it will restart the service

