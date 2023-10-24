# Secure communications explained

XProtect Access integrations can be configured to use encrypted communications. The XProtect Access integration with CCure 9000 can encrypt communications between the XProtect Access service and the XProtect Event Server which is running the CCure XProtect Access MipPlugin, and between the XProtect Access service and victor web service.

!!! glass "3rd party certificates"
    The fully detailed process included here is for self-signed certificates. If you are using a third party certificate, from a commercial certificate provider, please skip ahead to step number two below.

The following steps will enable secure communications for this solution.

1. Install a root certificate on the same server that will host the CCure XProtect Access Service
2. Install a certificate on the victor web service host and configure the IIS server to use the certificate.
3. Configure the CCure XProtect Access Service to use a certificate.
4. Configure the XProtect Access instance to use secure communications.

??? abstract "Learn more..."
    Please note that the instructions contained in this document are for generating your own certificates. It is also possible to obtain certificates from a trusted third-party certificate provider. For more information about certificates please read the [XProtect VMS certificates guide](https://doc.milestonesys.com/latest/en-US/portal/htm/chapter-page-certificates-guide.htm).