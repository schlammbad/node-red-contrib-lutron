# node-red-contrib-lutron
Node for Lutron HomeWorks devices on node-red

# Configuration
During configuration of the Lutron node you have to provide the IP address of the Lutron HomeWorks device.

The 2nd part of the configuration is to enter the switch ID and map it to a name.
I did not find any clean way to query the device ID to name mapping form the HUB so it's a manual step.

To identify the device ID to name mapping you can create a status node with DEVICE set to "ALL", connect the output of this node to a debug node and it will show you all the devices as they change status.
After this you can flip any of the device on this hub and it will show you ID for the device.
