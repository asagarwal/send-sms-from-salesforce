// Trigger on Case. This will call the Apex Class to send SMS and log it as an Activity
trigger caseTrigger on Case (after insert) {
      sendCaseSMS.callSMSService(trigger.newMap.keySet()) ;
}