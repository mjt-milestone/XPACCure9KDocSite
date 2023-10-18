# Scalablity and compatibility limits

Listed below are all of the compatibility and scalablity limitations built into the CCure XProtect Access integration.

## Software version compatibility

??? warning "CCure 9000 Version 3.0?"
    Version 3.0 of the CCure 9000 software is not supported by any version of the XProtect Access integration. The current version of the integration (1.4) supports all compatible versions of the CCure 9000 system. Older versions of the integration (1.3 and below) do not support any versions of the CCure 9000 software higher than 2.9 SP5.

Integration with CCure 9000 Access Control system is supported with all XProtect VMS products which can support MIP integrations and with a rules system that supports the XProtect Access suite of functionality.

The most up to date compatibility information is located here:

[Compatibility Statement](https://download.milestonesys.com/ccure9kxpa/CCure9000-XProtect-Access-Compatibility.pdf)

!!! glass "Version recommendations"
    Please confirm you have met the license requirements, and verify the version of CCure 9000 you are running is compatible. Milestone always recommends that you run the latest compatible versions of both CCure 9000 and XProtect.

## Hardware support

The following CCure 9000 panels have been tested and are known to be supported.

| Panel Model   | Description   |
|---------------|---------------|
| USTAR008      | iStar Ultra   |

!!! glass "Best practice"
    Verify your installation’s panel model numbers against this list, if one of your panels is not contained in this list, please contact your integrator and/or Milestone support to verify compatibility.

## Events handled

Current tests with CCure XProtect Access version 1.3 show a sustained rate of 75 events per second, with peak levels of performance measured at 125 events per second.

## Cardholders

The CCure 9000 XProtect Access integration should support any number of cardholders. However, XProtect Access has officially supported limitations for many system parameters. You can find those limitations listed in the most recent version of the XProtect Access Specification Sheet.