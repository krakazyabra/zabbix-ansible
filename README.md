# zabbix-ansible

Ansible playbook для добавления хостов в Zabbix Server

1. В веб-интерфейсе Zabbix сервера создать нового пользователья, от имени которого будет работать Ansible
2. В файле inventories/zabbix_hosts указать необходимые хосты, указать, какие шаблоны использовать для группы или конкретного хоста
3. В файле zabbix-host.yaml прописать ранее созданного пользователя и адрес сервера Zabbix
