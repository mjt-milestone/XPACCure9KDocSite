# CCure 9000 XProtect Access instance not displayed in XProtect Management Client

If XProtect is unable to communicate with the CCure 9000 XProtect Access instance, the instance will not appear in the access control section of the Management Client.  Do the following steps in the following order:

1. Close the Management Client and Smart Client.
2. Stop the XProtect Event Server.
3. Stop the Milestone XProtect Access Service.
4. Ensure CCure 9000 is running successfully. This may require restarting services.
5. Start the Milestone XProtect Access Service.
6. Start the XProtect Event Server and wait for it to fully start.
7. Start the Management Client.

If the instance still does not appear in the Management Client, investigate the logs (see [Using the log viewer application](../TC/Tray.md#using-the-log-viewer-application)) to discover the specific cause.