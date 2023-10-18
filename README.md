# Zabbix Templates for Intelbras's network devices

### Author: Arthur Cadore M. Barcella
#### Network Training Analyst at Intelbras

This repository is dedicated to [Zabbix's Template](https://www.zabbix.com/documentation/current/en/manual/config/templates) files for Intelbras network products. 

---
How to Use the Repository:

First clone this repository to your local machine using the following command:

```
git clone https://github.com/arthurcadore/ZabbixTemplates
```

Locate Your Template (.json file):

Navigate to the appropriate folder in the cloned repository to find the Zabbix template corresponding to your network product.

--- 

Import into Zabbix:

It's recommended to create the following Host Groups on Zabbix before importing the files: 

- OLT: `OLT Intelbras - Capacitação Redes`
- Switches: `Switches Intelbras - Capacitação Redes`
- Wireless Indoor: `Wireless Indoor Intelbras - Capacitação Redes`
- Wireless Outdoor: `Wireless Outdoor Intelbras - Capacitação Redes`


Log in to your Zabbix web interface.
Navigate to `Configuration` -> `Templates` in the left menu.
Click on the `Import` button.
Choose the downloaded Zabbix template file (ending in .json) from your local machine.
Click `Import` to add the template to your Zabbix environment.


--- 

Apply Template:

After importing, go to `Configuration` -> `Hosts` and select the host you want to monitor.
In the `Templates` tab, click `Select` and add the imported template to the host. Save your changes. 

Remember that: The template uses SNMP to collect the device's information, so it's important to have SNMP enabled on your device before adding it to Zabbix!
