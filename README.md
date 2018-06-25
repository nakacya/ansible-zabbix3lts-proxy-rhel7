
# Installation for Zabbix3LTS

clone repository
```
git clone https://github.com/nakacya/ansible-zabbix3lts-proxy-rhel7.git
```

configuration
```
vim ./ansible-zabbix-rhel7/group_vars/zabbix3lts-proxy-server-mysql
```

place of installation
```
vim ./ansible-zabbix3lts-proxy-rhel7/hosts
```

execute
```
cd ansible-zabbix3lts-rhel7
ansible-playbook -u <userName> ./zabbix3lts-proxyr-mysql.yml

# public key authentication
ansible-playbook --private-key=<pathToPrivatekey> -u <userName> ./zabbix3lts-proxy-mysql.yml
```

mysql security setting
```
mysql_secure_installation
```

First time login
```
http://<ipAddress or DNS>/zabbix/
user: Admin
pass: zabbix
```
#ansible-zabbix3lts-rhel7
