# Smart Client system error with StateCode: LicensedQuantityReached

A system error can occur in CCure with the following error code:

**LicenseQuantityReached**

“The option Milestone XProtect Corporate is licensed for 1 connections and that limit has been exceeded.”

This error is caused by a known bug in versions of CCure equal or prior to 2.80 SP1 that prevents the integration from connecting more than once to the CCure victor web service. The integration has been modified to recover from this error automatically when it occurs, but the recommended solution is to update CCure to a service pack higher than the above-mentioned versions.