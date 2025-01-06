### Steps

1. Start Elastisearch in cloud.elastic.co via free trial account, then create a deployment.
<img src="https://github.com/scalmueti/Log-Analysis-and-Threat-Detection-with-ELK-Stack/blob/main/Screenshots/Step%201_Make%20elastic%20Account.png?raw=true"><br>
Proof of account creation and Elastic Cloud deployment created.

2. Install the Kibana integration via search bar, then install Elastic Agent onto host computer.
<img src="https://github.com/scalmueti/Log-Analysis-and-Threat-Detection-with-ELK-Stack/blob/main/Screenshots/Step2_Install%20Kibana.png?raw=true"><br>
After searching for Kibana in the search bar at the top and clicking "Add item..."

2.1. After running the provided command, go back to the Elastic Cloud window and confirm settings
<img src="https://github.com/scalmueti/Log-Analysis-and-Threat-Detection-with-ELK-Stack/blob/main/Screenshots/Step2_1_Integration%20confirmation.png?raw=true"><br>
Confirmation screen after Elastic Agent was installed.

2.2. Once the settings and Elastic Agent all work, confirm the data that is incoming to Elastic Cloud.
<img src="https://github.com/scalmueti/Log-Analysis-and-Threat-Detection-with-ELK-Stack/blob/main/Screenshots/Step2_2_ConfirmConnection.png?raw=true"><br>
Shows data that is being processed by the Elastic Agent and sent to Elastic Cloud.

2.3. Confirm the Kibana integration instance by managing the deployment.
<img src="https://github.com/scalmueti/Log-Analysis-and-Threat-Detection-with-ELK-Stack/blob/main/Screenshots/Step2_3_InstanceConfirm.png?raw=true"><br>
Kibana instance is confirmed in the management settings.

3. Install Sysmon onto the host computer to get readable and useful Windows logs.
<img src="https://github.com/scalmueti/Log-Analysis-and-Threat-Detection-with-ELK-Stack/blob/main/Screenshots/Step%203%20Install%20Sysmon.png?raw=true"><br>
Proof of Sysmon being installed via Powershell command.

3.1. Setup the Windows integration in Elastic Cloud with the current Elastic Agent.
<img src="https://github.com/scalmueti/Log-Analysis-and-Threat-Detection-with-ELK-Stack/blob/main/Screenshots/Step3_1.png?raw=true"><br>
Search for the Windows integration via the search bar in Elastic Cloud. (It is important to configure it correctly to use the previous agent policy.)

3.2. Confirm the Windows integration setup with the Elastic Agent client.
<img src="https://github.com/scalmueti/Log-Analysis-and-Threat-Detection-with-ELK-Stack/blob/main/Screenshots/Step3_2.png?raw=true"><br>
Proof of the Windows client working with the integration.

3.3. Using the following filter, "data_stream.dataset is windows.sysmon_operational" to filter out the Sysmon logs and view them in Elastic Cloud.
<img src="https://github.com/scalmueti/Log-Analysis-and-Threat-Detection-with-ELK-Stack/blob/main/Screenshots/Step3_3.png?raw=true"><br>
Shows the filter working on the log reports, showing only Sysmon logs.
