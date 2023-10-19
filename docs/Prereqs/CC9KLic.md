# CCure 9000: licenses explained

Licenses required for CCure 9000 change based on the version of software installed. For versions 2.9 SP5 and below, there are two licenses required. For versions 2.9 SP6, 3.00.1 and above there is only one license required. These licenses aren't compatible. If you are upgrading to 2.9 SP6 or 3.00.1, contact CCure for the new license.

??? warning "Corporate license?"
    The CCure 9000 license required to integrate with Milestone XProtect is “Milestone XProtect Corporate” or "Milestone - XProtect Corporate." This doesn't mean that the only XProtect product that integrates with CCure 9000 is XProtect Corporate. XProtect Corporate, XProtect Expert, and XProtect Professional+ VMS products from Milestone are all tested and supported

There are three different types of **Milestone XProtect Corporate** licenses based on the size of the CCure system (the number of readers). These license options apply to all versions of CCure 9000.

| License SKU   | Description   |
|---------------|---------------|
| CC9-MSTVD-SM  | CCure 9000 Milestone XProtect Corporate Web Service Integration Small, Series L to N (0-64 readers)   |
| CC9-MSTVD-MD  | CCure 9000 Milestone XProtect Coporate Web Service Integration Medium, Series P to R (65-999 readers) |
| CC9-MSTVD-LG  | CCure 9000 Milestone XProtect Corporate Web Service Integration Large, Series RP to T (1000+ readers) |

XProtect Access uses a permanent connection to the CCure 9000 victor web service (to receive statuses and events) and uses extra connections for specific user operations, such as fetching configuration and executing commands. For optimal operation of XProtect Access, the feature license activated in CCure must support enough concurrent connections to the victor web service to handle the number of XProtect Access permanent and transient connections.

!!! glass "victor web service license"
    The victor web service is a requirement for the XProtect Access integration with CCure 9000. However, if you aren't running version 2.9 SP6 or 3.00.1 of CCure, this licensed option is typically included.

## CCure 9000 version 2.9 SP6 and 3.00.1 licenses

In CCure 9000 versions 2.9 SP6 and 3.00.1 the license requirements change. The only required license is:

+ **Milestone - XProtect Corporate**

This is a web service license, therefore it includes the victor web service component. Below is the process for applying this new license.

1. Once you have received the license file (.TLIC), move it to the CCure 9000 server.
2. Open the **License Manager** application and add the .TLIC file as a new license.
3. Reboot the server, or restart the CrossFire services to apply the license.
    + **CrossFire Framework Service**
    + **CrossFire Server Component Framework Service**
4. Verify license application by checking the **Options** menu of the **License** tab in the **Help | About** menu of the CCure Administration Station

!!! glass "How to tell the different licenses apart?"
    The license must display the available concurrent connections for the web service. [0/10]</br>
    </br>
    ![One_Lic](img/CP3_0licenseverify.png){width=60%}

## CCure 9000 version 2.9 SP5 and below licenses

There are two feature licenses required in CCure versions 2.9 SP5 and below:

1. “Milestone XProtect Corporate” - this is an SDK license required for the integration.</br>
    </br>
    ![Corp_Lic](img/Prerequisites.png){width=40%}</br>
2. “victor web service” - this license enables the web server functionality to communicate with XProtect Access.</br>
    </br>
    ![vws_Lic](img/Prerequisites_1.png){width=40%}</br>
