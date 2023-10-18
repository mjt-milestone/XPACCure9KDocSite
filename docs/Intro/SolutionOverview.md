# Solution overview

The integration software download is a single context sensitive installation program. This program name is:

**XProtectAccess.CCure9k.msi**

When this program runs it identifies the software installed on the local server, CCure 9000 or XProtect, and it helps install the required software. One of these two options are presented:

1. The CCure XProtect Access Service that runs on the CCure 9000 server.
2. The CCure XProtect Access MipPlugin that runs on the XProtect server.

**Single system: XProtect Access Service and CCure 9000 software on the same host.**

``` mermaid
flowchart LR
    a("CCure XProtect Access MIP Plugin"):::XPClass -- "HTTPS" --> b("CCure XProtect Access Service"):::XPClass
    b("CCure XProtect Access Service"):::XPClass ---> a("CCure XProtect Access MIP Plugin"):::XPClass
    subgraph "CCure 9000 Server"
    b("CCure XProtect Access Service"):::XPClass <--> c("victor web service"):::XPClass
    end
    subgraph "XProtect Management Server"
        direction TB
        subgraph "XProtect Event Server Process"
        a("CCure XProtect Access MIP Plugin"):::XPClass
        end
    end 
    classDef XPClass fill:#efb, stroke:#000, stroke-width:2px
```

!!! warning "Version dependency!"
    The versions of the CCure XProtect Access MIP Plugin and the CCure XProtect Access Service which are installed and running in the system must be the same identical versions or the integration will not work.