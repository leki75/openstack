All-in-one deployment on Vagrant
================================

* Copy all-in-one configuration file
  $ ../scripts/restorecfg.sh aio-file
* Generate secrets
  $ ../scripts/generate_secrets.py
* Ensure that network configured in ./Vagrantfile is the same as in 
  ../inventory/inventory.yml and vip addresses are on the same network 
  in ../group_vars/all/config.yml
* Start deployment
  $ vagrant up

It is possible to rerun the deployment with 'vagrant provision' if
something failed.
