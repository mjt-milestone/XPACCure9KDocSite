# XProtect Access instance connection properties

The credentials and parameters required to connect the XProtect Access instance to the CCure 9000 system are detailed below:

| Property Name | Required Entry Details    |
|---------------|---------------------------|
| Name  | Custom name field  |
| Integration plug-in  | Displays the current version of the ACM MIP Plugin  |
| XProtect Access Service Host  | [ Hostname.Domain.TLD ] This field should contain the Fully Qualified Domain Name (FQDN) of the CCure 9000 server where the XProtect Access Service was installed.   |
| XProtect Access Service Port  | 8443 is the default  |
| XProtect Access Service - SSL Certificate Validation  | Enables SSL certificate validation between the CCure XProtect Access Service and the CCure XProtect Access MipPlugin. This option is required to use a third party certificate. Not enabled by default.  |
| Victor Web Service - Host  | Host name of the CCure 9000 server.  |
| Victor Web Service - Port  | 443 is the default  |
| Victor Web Service - Use HTTPS  | HTTPS is required for secure connection to CCure 9000 by default  |
| Victor Web Service -SSL Certificate Validation  | Enables SSL certificate validation between the CCure XProtect Access Service and victor web service when a third party certificate is being used. Not enabled by default.  |
| Victor Web Service - User  | [ Domain\Username ] for a user account with administrative privileges on the CCure 9000 server.  |
| Victor Web Service - Password  | Password for the user account selected for the “Username” field.  |
| Options – States polling interval (seconds)  | Default value is 900 seconds. Frequency of status updates retrieved for access control hardware devices.  |
| Options - [Legacy] Connection Profile  | 	Used for backward compatibility with previous versions of the integration (after an upgrade). In most cases, this field must be empty.  |
| Options – Enable performance metrics (diagnostics)  | Not selected by default. Select this option to include performance statistic logging on event metadata.  |

!!! warning "Encryption requirements"
    The **Victor Web Service - Host** field must contain the PC name of the server where the victor web service is installed. The script used to create the certificate specifies the PC name and any other method of identification for the server - such as the IP address or the fully qualified domain name - will not work. Make sure to match the PC name from the script with the data entered in the **Victor Web Service - Host** field.