# Satellite 6.x Inventory Report Instructions

In order to export the inventory from Satellite version 6 please follow the instructions
below.

1. Download the Sat6 Inventory Script from Github.
[https://github.com/RedHatSatellite/sat6Inventory/archive/master.zip](https://github.com/RedHatSatellite/sat6Inventory/archive/master.zip])
2. Extract the script to a workstation or server that has Python >= 2.6.
3. From the workstation or server where the script has been extracted run the script with the following options (replacing {SATELLITE} with the FQDN of the Satellite 6 server, and {admin} with the admin user name for your satellite server.
```
./sat6Inventory.py -s {SATELLITE} -l {admin} -f \
spacewalk-report-inventory-customized
```
4. The script will prompt you for the password of the user you provided and will save the results in the same folder in a file named all_inventory_report.csv.
5. If the script does not complete properly you can use the -d option to enable debug mode.


See this Github document for additional information - [https://github.com/RedHatSatellite/sat6Inventory/ (https://github.com/RedHatSatellite/sat6Inventory/)
