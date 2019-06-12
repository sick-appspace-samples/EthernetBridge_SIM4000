## EthernetBridge_SIM4000
Using Ethernet bridge on SIM4000 to change IP-Address of attached pico-/midiCams
### Description
This SampleApp shows how to adapt IP-Address of 2 pico-/midiCams using the
SICK-I2DCameraManager without disconnecting the cameras from the SIM4000.
In the same way IP addresses of SICK sensors can be modified using SOPAS-ET instead. Note: This SampleApp requires SIM4000 FW1.5.0 or higher.
### How to Run
In order to work the following steps have to done in the exact order
0.  Deactivate all running Apps
1.  Activate EthernetBridge-App in the AppExplorer of AppStudio
2.  Start the App with "Run all Apps" and wait for EthernetBride "running" state in the AppMonitor
3.  Start the I2D Camera Manager and activate "Expert-Mode"
     The two cameras connected at ETH2/3 should appear in the Camera List (ignore the exclamation
     mark and the red text at the bottom of the camera manager window)
4.  Select a camera in the Camera List
5.  Select "Manual ETH Configuration"
6.  Type-in the required "Persistent IP" address of the camera and confirm with "OK"
7.  Repeat steps 3, 4 and 5 for the 2nd camera
8.  Stop Ethernet-Bridge-App typing "Stop all Apps" and wait for "No Apps running" state in the AppMonitor
     Note: Stopping the App takes some time and results in a connection loss
9. Reconnect to the SIM4000 and wait for EthernetBride  "stopped" state in the AppMonitor
10. Deactivate EthernetBridge-App in the AppExplorer time and wait for "No Apps running" state in the AppMonitor
11. Activate and start any other App

### Topics
Device, SIM4000, Communication, Sample, SICK-AppSpace