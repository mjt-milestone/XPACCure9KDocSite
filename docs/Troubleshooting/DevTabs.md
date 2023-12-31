# XProtect Access developer tabs (explained)

Hidden tabs are built into the XProtect Access instance in the Management Client. These tabs contain helpful information when troubleshooting.

![Dev_Tab_GUI](img/CX.DevTabEXP.png){width=75%}

## Enabling developer tabs

Take these steps to enable the hidden developer tabs built into the XProtect Access instance.

1. Select **Options** from the **Tools** menu of the Management Client.
2. Go to the **Access Control Settings** tab of the Options dialog and select the **Show development property panel** option.

![Tools_Options_Enable](img/CX.showDEV.png)

## Developer tabs (reference)

Below is a description of how to use each of the hidden developer tabs available within the XProtect Access instance.

=== "DEV:Info"    
    | Tab Name  | Description   |
    |-----------|---------------|
    | DEV: Info  | 	This tab has the entire hierarchy of servers, devices, statuses, commands, and events in the system. Selecting an individual object allows for identification of any properties associated to it.   |</br>

    ![DEV:Info](img/CX.DevInfo.png){width=75%}

=== "DEV:Item States & Commands"    
    | Tab Name  | Description   |
    |-----------|---------------|
    | DEV: Item States & Commands  | 	This tab shows all devices and servers in the system. Select a device or server to view all associated commands and possible statuses. The current state of the device or server is displayed in bold.   |</br>

    ![DevItemStates](img/CX.DevDeviceStates.png){width=75%}

=== "DEV: Category Mapping"  
    | Tab Name  | Description   |
    |-----------|---------------|
    | DEV: Category Mapping  | 	The Category Mapping tab is primarily used for debugging during development making sure that the Events, Commands, States, Servers, and Devices are mapped correctly between CCure and XProtect.   |</br>

    ![DEV:CatMap](img/CX.DevCatMaps.png){width=75%}

=== "DEV: Camera Mapping"    
    | Tab Name  | Description   |
    |-----------|---------------|
    | DEV: Camera Mapping  | 	This tab displays the current camera to device mapping used in the XProtect Access instance.   |</br>

    ![DEV:CamMap](img/CX.DevCamMap.png){width=75%}

=== "DEV: Live Events"
    | Tab Name  | Description   |
    |-----------|---------------|
    | DEV: Live Events  | 	This tab will display live events as they're received by the XProtect Access system when selected. If the client is closed, or the user switches to another view, the Live Events tab won't retain any memory of the events displayed. This memory-less behavior is something all three Live tabs have in common.   |</br>

    ![DEV:LiveEvents](img/CX.DevLiveEvents.png){width=75%}

=== "DEV: Live State Changes"    
    | Tab Name  | Description   |
    |-----------|---------------|
    | DEV: Live State Changes  | 	This tab displays the live status changes of devices and servers. This tab has no memory.   |</br>

    ![DEV:LiveState](img/CX.DevLiveState.png){width=75%}

=== "DEV: Live Credential Holder Changes"
    | Tab Name  | Description   |
    |-----------|---------------|
    | DEV: Live Credential Holder Changes  | 	This tab shows all credentials added to the XProtect Access system. This tab has no memory.   |</br>

    ![DEV:LiveCreds](img/CX.DevLiveCreds.png){width=75%}
***