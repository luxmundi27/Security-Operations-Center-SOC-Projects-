# SECURITY-OPERATION - CENTER (SOC Projrcts and labs)
## Security Operations Center labs, SIEM engineering, detection engineering, and threat hunting projects.

# (Lab1) 
# Windows Event Monitoring Using Splunk in A Simulated SOC Lab

### SOC lab without Splunk, each component generate and keeps its logs
<img src="Resources/Splunk.png" alt="Lab image">

## Project Objectives
To simulate a basic SOC environment by collecting and monitoring system logs using Splunk ES, and creating arlets for potential security incidents( Brute force attempts, failed logins etc), create an vizualizse results on dashboards.
### SOC Labs with Splunk Forwarders ingesting logs to Splunk ES
<img src="Resources/Forwarders.png" alt="lab image with forwarders"> 

### Tools Used
- Splunk ES (installed locally)
- Splunk Forwarders (Installed on VMs)
- Windows 10 VM with Sysmon installed
  ### Project Task and Steps
  ### A) Set up Splunk ES
  - Installed Splunk locally
  - Create a Splunk Admin account
  -  Enable port 8000 access
  ### B) Installed and configured Sysmon on windows
  - Used SwiftOnSecurity Sysmon cofiguration
  - Log key activities like process creation, network connection, file creation
  ### C)  Forward Logs to SplunK
  - Used Splunk Universal Forwarders to collect logs from VMs to Splunk ES
  - Index and Tag Log sources as Windows and Sysmon
  ### D) Create Dashboards
  ### E) Set Detection Alerts
  ### F) Simulate Attacks
  ### G) Document Your Findings

-------------------------------------------------------------------------------------------------------------------------------
# 2) Brute-Force-Detection-App-using-Python-Streamlit
## Screenshots 
## Before
<img src="https://github.com/luxmundi27/Brute-Force-Detection-App-using-Python-Streamlit/blob/main/Brute%20force.png" alt="Lab image">

## After : Checking if an IP has been Brute-Force
<img src="https://github.com/luxmundi27/Brute-Force-Detection-App-using-Python-Streamlit/blob/main/Brute%20forece%202.png" alt="Lab image">


## Objective
Develop a user-friendly application that helps identify potential brute-force attacks by analyzing system logs for patterns of repeated failed login attempts, access anomalies, or suspicious user behavior.
## Problems Solved
•	Intrusion Detection: Flags excessive failed login attempts suggesting brute-force attempts

•	Real-time Monitoring: Enables tracking live logs or periodic scans for login abuse

•	User Behavior Analysis: Offers insights into login frequency, timing, and IP activity

•	Learning Platform: A safe space to explore brute-force detection concepts without engaging in malicious activities
## Tools & Technologies Used
|Tool	      | Role                                                        |
|-----------|-------------------------------------------------------------|
|Python 	  |Core backend scripting for data analysis                     |
|Streamlit  |Builds an intuitive and interactive front-end UI             |
|pandas:  	|Parses and analyzes log files efficiently                    |
|re (Regex) |Detects suspicious patterns like repeated failed attempts    |
|datetime 	|Tracks timestamps and calculates time-based anomalies        |
|socket 	  |Optionally resolves IP addresses and ports (for advanced use)|
## Features
•	Log File Upload: Accepts system-auth or custom logs for analysis

•	Alert System: Visual flags when brute-force patterns are detected

•	Stats Dashboard: Number of failed attempts, flagged IPs, peak attack times

•	IP Lookup (Optional): Resolve locations or blacklist common sources
## Sample Use Cases
•	Educational labs in cybersecurity classes

•	Internal tool for sysadmins to audit login security

•	Prototype module for larger SIEM systems
