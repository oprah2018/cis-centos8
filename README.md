# cis-centos8

Prereqisition
 * [install ansible]
 * make sure your ssh connections to your cluster are available

```
$ cp cis-centos8/inventory/mycluster.ini.template cis-centos8/inventory/mycluster.ini
```
edit your inventory files cis-centos8/inventory/mycluster.ini , then run

```
$ ansible-playbook -i cis-centos8/inventories/mycluster.ini cis-centos8/cis-centos8.yml -u root -k
```

# tmp

```
$ ansible all -m ping -i inventories/mycluster.ini -u root -k
```

# links
 * [template](https://github.com/radsec/CentOS7-CIS)
 * [cis benchmark](https://www.cisecurity.org/benchmark/centos_linux/)