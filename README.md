# zabbixTemplates

### Author: Arthur Cadore M. Barcella
#### Network Training Analyst at Intelbras

This repository is dedicated to zabbix's Template files for Intelbras network products. 

---
How to Use the Repository:

First clone this repository to your local machine using the following command:

```
git clone https://github.com/arthurcadore/zabbixTemplates
```

Locate Your Template (.json file):

Navigate to the appropriate folder in the cloned repository to find the Zabbix template corresponding to your network product.

--- 

Import into Zabbix:

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
