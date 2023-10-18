# Alarm acknowledgment - explained

Bi-directional alarm/event acknowledgment is supported between XProtect and CCure 9000.

??? glass "Video Push?"
    In some scenarios, acknowledging alarms in the XProtect Smart Client may not automatically acknowledge the alarms in the CCure system. In systems using both integrations: (i.e. the XProtect Access integration with CCure and the Video Push CCure integration) – XProtect analytics alarms generated by the Video Push CCure integration only support automatic acknowledgment if they are acknowledged in the CCure Monitoring Station application, and the **Auto-acknowledge alarms** option was selected in the CCure event definition.

1. CCure 9000 to XProtect:</br>
    + When a CCure 9000 event is acknowledged, if an alarm was triggered in XProtect that matches that event, the XProtect alarm will be acknowledged.</br>
2. XProtect to CCure 9000:</br>
    + When an alarm is acknowledged in XProtect, the event in CCure 9000 that triggered the alarm will also be acknowledged.
    + When using the XProtect Smart Client’s **Alarm Manager** tab, right-click an alarm, and select **Acknowledge**. The associated CCure 9000 event will be acknowledged.

??? glass "Close or Acknowledge?"
    Acknowledging an alarm in XProtect will acknowledge the alarm in CCure. Closing an alarm in XProtect will not acknowledge the alarm in CCure 9000. Only acknowledgment of the alarm in XProtect will impact the alarms status in CCure 9000.