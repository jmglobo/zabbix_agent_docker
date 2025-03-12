# ZABBIX AGENT

Docker compose witch contains a Zabbix agent that run in Linux machine and can comunicte with your Zabbix server.

This way you don´t need configure a zabbix agent in your Linux machine. You only need to have:
- Docker
- Docker-compose

The configuracion is really easy:
- ZBX_HOSTNAME= Put the hostname machine which you have put in you Zabbix server for this machine
- ZBX_SERVER_HOST= You need indicate the IP belong to machine (or container) who runs Zabbix server  
- ZBX_ACTIVE_SERVERS= You need indicate the IP belong to machine (or container) who runs Zabbix server   
- ZBX_LISTENPORT= Port of your machine who runs this compose. Port 10052 is highly recommended
- ZBX_SERVER= You need indicate the IP belong to machine (or container) who runs Zabbix server   

The 'network_mode : host' means the machine don´t will create another network for this container. This way is far easy than install a Zabbix agent.
