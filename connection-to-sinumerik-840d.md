#### Siemens Sinumerik 840d connection configuration

dataFEED edgeConnector Siemens provides an interface to connect and
fetch data from the Siemens SINUMERIK 840D series.

To configure a Siemens SINUMERIK 840D connection, navigate to
**Connectivity-\>PLC-\>Siemens SINUMERIK 840D** as depicted in the
navigation tree below:

![sinumerik 840d_navigatiin](documentation_pics/image154.png)  

 The page provides an overview of the currently configured connections including the `Name`, the `IP address`, the connection `Status` and the `Enabled` state.  
![sinumerik 840d_overview](documentation_pics/image155.png)  


| Column name | Information details |
| :-- | :-- |
| Name | Connection name as defined at creation time. |
| IP Address | IP Address or host name of the PLC |
| Status | Describes the state of the PLC connection; can be either Connected when the connection to the PLC is established or Disconnected when there is no connection to the PLC. The connection status is dynamically updated each 2 seconds. |
| Enabled | Describes the configuration state of the PLC connection. Possible values are Enabled or Disabled. Note: Clicking on the current configuration state icon would trigger a state toggle: Enabled -> Disabled ; Disabled -> Enabled |  


From the title bar of the connection overview table a new connection can be added and existing connections can be either edited or deleted.  
To add a new connection cklick the ![add_connection](documentation_pics/add_connection.png) button.  
To edit an existing connection, first select it from the overview table and click the ![edit_connection](documentation_pics/edit_connection.png) button.  
To delete an existing connection, first select it from the overview table and click the ![delete_connection](documentation_pics/delete_connection.png) button.  

Adding a new connection and editing an existing connection, each open the same page. The only difference is, that for an existing connection the `Connection Name` property can not be changed.  
The `Connection Name` must be unique and can only be assigned when adding a new connection.  
The state of `Enabled` checkbox determines if the connection shall be used.  
The `PLC Address` holds the address of the target device (Sinumerik 840d). This is either an IP address or a hostname.  

#### Siemens Sinumerik 840d connection advanced configuration

![Advanced 840d connection configuration page](documentation_pics/s480d-advanced-settings.png)

The advanced configuration page of 840d connection allows to change the following settings:

  1. **Destination port:** This should remain on the default value 102.
  2. **NCK TSAP Selection:** This allows to switch between the TSAP for "Simatik 840D SL" and a user defined TSAP.
      This setting should only be changed, if a connection to "Simatik 840D PL" or other none Solution Line series device
	  is desired.
  3. **User-Defined:** Input field for customized TSAP setting. Allowed input are hexa-dezimal diggits. E.g.:
     - `02 01`
	 - `2 1`
	 - `0201`
  4. **PLC TSAP Selection:** This allows to switch between the TSAP for "Simatik 840D SL" and a user defined TSAP.
      This setting should only be changed, if a connection to "Simatik 840D PL" or other none Solution Line series device
	  is desired.
  5. **User-Defined:** Input field for customized TSAP setting. Allowed input are hexa-dezimal diggits. E.g.:
     - `02 01`
	 - `2 1`
	 - `0201`
  6. **Enable NCU Alarm:** This checkbox enables or disables the subscriptions of NCU alarms from the Simatic 840D.