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


Default username and password are:
 - username: opendcim
 - password: opendcim

If you want to load a database backup, make sure you have a file called `dump.sql.bz2` in the playbook folder. If the file is present the database backup will be installed.

If you load a database backup, please note that objects in the database bring with them the information about the user that created them. Edit the file `vars/main.yml` and edit `webuser` with a value that is coherent with your database backup.
