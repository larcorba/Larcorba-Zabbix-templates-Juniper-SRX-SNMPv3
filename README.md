Zabbix template
======

Intro
------
Check out Zabbix share and drop a rating/comment! :)

https://share.zabbix.com/network_devices/juniper/juniper-srx-snmpv3-general


Features
------
- Interface discovery
  - Logical interface discovery possible but disabled
  - Optical dBm Values
- Hardware discovery
- New flow per second graphs
- Inventory field items


Macros
------
Do not forget the add the macro's:

User: {$JUN_V3_USER}

Password: {$JUN_V3_AUTHPASS}


Inventory
------
Make sure to add the inventory 'automatic' options at your host if you want to use the invetory option.


Logical interface disovery
------
^(fe|ge|xe|et)-[0-9]+\/[0-9]+\/[0-9]+\.[0-9]+$|^(fe|ge|xe|et)-[0-9]+\/[0-9]+\/[0-9]+$|^(reth|st)[0-9]+\.[0-9]+$|^(reth|st)[0-9]$|^vcp-[0-9]+$|^vlan.[0-9]+$

or

^(fe|ge|xe|et)-[0-9]+\/[0-9]+\/[0-9]+$|^(fe|ge|xe|et)-[0-9]+\/[0-9]+\/[0-9]+$|^(reth|st)[0-9]+$|^(reth|st)[0-9]$|^vcp-[0-9]+$|^vlan.[0-9]+$
