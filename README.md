# Wazuh-SIEM-SOC-Lab
## Project Overview
This project documents the deployment and configuration of a Wazuh Security Information and Event Management (SIEM) environment for hands-on Security Operations Center (SOC) training.

The lab focuses on endpoint security monitoring, log collection, threat detection, security event analysis and incident investigation

## Project Objectives
- Deploy and configure Wazuh SIEM.
- Integrate Windows and Linux endpoints.
- Collect and analyze security event logs.
- Configure Windows Sysmon for enhanced monitoring.
- Investigate failed authentication attempts.
- Develop custom security detection rules.
- Practice SOC alert triage and incident investigation.

## Lab Environment

| Component  |  Technology |
--------------|---------------|
| SIEM Platform | Wazuh     |
| SIEM Server  | Ubuntu Server |
| Virtualization | VMware |
| Windows Endpoint | Windows 10 |
| Linux Endpoint | Ubuntu Linux Endpoint |
| Endpoint Monitoring | Wazuh Agent |
| Windows Telemetry | Sysmon |
| Log Analysis | Wazuh Dashboard |

## Implementation

The project documentation will cover the following:

### Phase 1: Wazuh Server Deployment
### Wazuh Manager Service Verification
After deploying the Wazuh manager on Ubuntu, I verified that the service was running successfully.

**Command executed:**
```bash
sudo systemctl status wazuh-manager
```
***Verification Results:**
- Wazuh Manager service was active and running.
- The service was enabled.
- Wazuh analysis engine processes were running.
- Wazuh log collector processes were running.
- Wazuh API processes were running.
  
**Evidence:**

![Wazuh Manager Service Status](Screenshots/wazuh-manager-status.png)

**Security Relevance:**

The Wazuh Manager is responsible for processing security events collected from monitored endpoints and evaluating them against configured detection rules. 
Verifying its operational status is an important step in maintaining a functional SIEM environment.
  

### Phase 2: Endpoint Integration 
Deployment of Wazuh agents on Windows and Linux endpoints.

### Phase 3: Windows Sysmon Integration 
Configuration of Sysmon to collect detailed Windows telemetry.

### Phase 4: Security Event Monitoring 
Monitoring Windows authentication events, account activity and other security events.

### Phase 5: Custom Detection Rules 
Creating and testing Wazuh detection rules for suspicious security activities.

### Phase 6: Security Investigation 
Analyzing security alerts and documenting investigation findings

## Project Screenshots 
Screenshots demonstrating the implementation, configuration and security monitoring activities will be added as the project documentation

