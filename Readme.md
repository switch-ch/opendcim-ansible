# README

To test the playbook with vagrant,
start the Vagrant virtual machine

```
vagrant up
```

Run the ansible playbook
```
ansible-playbook opendcim.yaml -i vagranthosts
```
you can point your browser at http://localhost:8080

If you want to load a dabase backup, make sure you have a file called `dump.sql.bz2` in the playbook folder. If the file is present the database backup will be installed

Default username and password are:
 - username: opendcim
 - password: opendcim
