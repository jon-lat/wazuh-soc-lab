# Wazuh SOC Home Lab

## Overview

This project is a home Security Operations Center (SOC) lab built to practice security monitoring, endpoint visibility, and security event investigation.
The lab uses Wazuh as a SIEM platform to collect and analyze security events from a Windows endpoint. The goal was to simulate basic SOC analyst workflows such as monitoring authentication activity and investigating endpoint events.

Wazuh Homepage:

![Wazuh Homepage](screenshots/wazuh-homepage.png)


Windows Agent Connection:

![Windows Agent](screenshots/windows-agent.png)


## Lab Setup

The lab consists of an Ubuntu Server VM running Wazuh and a Windows VM acting as a monitored endpoint. 

The Wazuh agent forwards Windows security logs to the SIEM dashboard for analysis.

## Detection Scenarios

### Successful Logon (Event ID 4624)

Correct Password entered by user in Windows login screen.

A successful authentication event was generated and analyzed through the Wazuh dashboard.

Screenshot:

![Successful Logon](screenshots/successful-login-event.png)


### Failed Logon (Event ID 4625)

Multiple wrong passwords were entered by user in Windows login screen.

Multiple failed authentication attempts were generated to simulate suspicious login activity.

Screenshot:

![Failed Logon](screenshots/failed-login-event.png)


### System Shutdown Event

Windows shutdown event was generated and analyzed through the Wazuh dashboard.

Screenshot:

![Shutdown Event](screenshots/shutdown-event.png)

## Skills Demonstrated

- SIEM deployment and configuration
- Endpoint monitoring
- Windows event log analysis
- Security event investigation
- Linux server administration
- Virtual machine networking
