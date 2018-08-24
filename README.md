# Добавление нового хоста в Zabbix, используя Ansible

zabbix-host.yaml - Ansible playbook для добавления хостов в Zabbix Server

1. В веб-интерфейсе Zabbix сервера создать нового пользователья, от имени которого будет работать Ansible
2. В файле inventories/zabbix_hosts указать необходимые хосты, указать, какие шаблоны использовать для группы или конкретного хоста
3. В файле zabbix-host.yaml прописать ранее созданного пользователя и адрес сервера Zabbix

# Установка Zabbix агента на Ubuntu/Debian
zabbix-agent.yaml - Ansible playbook для

а. Установки Zabbix агента
б. Установки утилит (sysstat, bc, lm-sensors, sudo)
в. Добавления пользователя Zabbix в список sudoers
г. Копирования папки scripts и zabbix_agetd.d со всем содержимым
д. Установки необходимых для шаблона [Linux Disk Performance Monitoring](https://share.zabbix.com/storage-devices/linux-disk-performance-monitoring) файлов (скрипт обнаружения дисков и userconfig)

1. В файле zabbix-agent.yaml указать сервера Zabbix Сервера (или Zabbix Proxy)
2. В папку scripts положить необходимые скрипы (обычно идут вместе с шаблоном)
3. В папку zabbix_agetnd.d полопжить файлы конфигурации (обычно идут вместе с шаблоном)
