### SNMP Builder - SNMP MIB Import for Zabbix (1.8.12) Monitoring System

This repository contains files that are needed to add SNMP MIB Import functionality to Zabbix Monitoring System

#### Installation
1. Get SNMP Builder

   ```shell
   git clone -b 1.8.12 https://github.com/macrokernel/zabbix-snmpbuilder
   ```
2. Go to to Zabbix frontend directory on your Zabbix server

   ```shell
   cd /usr/share/zabbix
   ```
3. Copy snmpbuilder patch file and images archive to this directory
4. Apply snmpbuilder patch

   ```shell
   patch -p3 < zabbix-1.8.12-snmpbuilder.patch
   ```
5. Unpack images archive

   ```shell
   unzip zabbix-1.8.12-snmpbuilder-imgs.zip -d /usr/share/zabbix
   ```
6. Remove patch file and images archive

   ```shell
   rm zabbix-1.8.12-snmpbuilder.patch zabbix-1.8.12-snmpbuilder-imgs.zip
   ```
