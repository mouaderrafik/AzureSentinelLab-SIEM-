<h1>Azure Sentinel Lab - Log Failed RDP Attacks</h1>



<h2>Description</h2>
The Powershell script in this repository is responsible for analyzing Windows Event information related to RDP Brute Force (Remote Desktop Protocol) attacks. When working in conjunction with an open geolocation API and Azure Sentinel configured and connected to a virtual machine acting as a honey pot, it is able to show the geographic information of the attacks and their position on the Azure Sentinel world map.
<br />


<br />
<br />
<h3>Main points of the project:</h3>
<br />

- Development of custom PowerShell script to extract metadata from Windows Event Viewer and route to open source API to handle the data and show geolocation of events.<br /><br />
- Configuring the Log Analytics Workspace in Azure to insert custom logs containing geographic information (Latitude, Longitude, State and Country).<br /><br />
- Configuring custom fields in Azure's Log Analytics Workspace for mapping geographic data to Azure Sentinel.<br /><br />
- Configuring Azure Sentinel (Cloud SIEM) workbook to display global attacks (RDP brute force) on a map according to the location and magnitude of attacks.<br /><br />
- Criação e configuração de máquinas virtuais no Azure
<br />
<br />


<p align="center">
<img src="https://i.imgur.com/9iWaGkX.png" height="85%" width="85%" alt="RDP event fail logs to iP Geographic information"/>
</p>
<br />
<p align="center">
<img src="https://i.imgur.com/y0NVDHg.png" height="85%" width="85%" alt="RDP event fail logs to iP Geographic information"/>
</p>
<br />
<p align="center">
<img src="https://i.imgur.com/IaEG6b3.png" height="85%" width="85%" alt="RDP event fail logs to iP Geographic information"/>
</p>
<br />
<h2>Languages</h2>

- <b>PowerShell:</b> Extraction of the Windows Event Viewer Logon Logs

<h2>Utilities</h2>

- <b>ipgeolocation.io:</b> Returns geographic information for a given IP

<h2>Attacks from Panama being logged with geographic information</h2>

<p align="center">
<img src="https://i.imgur.com/xqMmXOW.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>World map showing latest RDP attacks recorded around the world with geographical information.</h2>

<p align="center">
<img src="https://i.imgur.com/1OrJxcT.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>
