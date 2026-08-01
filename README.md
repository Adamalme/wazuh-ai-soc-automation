# Wazuh AI SOC Automation

## What This Does
Python script that connects to Wazuh SIEM API and OpenSearch,
pulls real security alerts and uses OpenAI GPT to automatically
analyze each threat.

## Features
- Connects to Wazuh API automatically
- Pulls real security alerts from OpenSearch
- AI analyzes each alert with MITRE ATT&CK mapping
- Generates risk scores and recommended actions
- Saves full report to JSON automatically

## Tools Used
- Python 3
- Wazuh SIEM 4.14.7
- OpenSearch
- OpenAI GPT
- MITRE ATT&CK Framework

## Setup
1. Install Wazuh Manager on Linux
2. Configure Windows agent
3. Add your API credentials
4. Run: python wazuh-AI-agent.py
AI-powered Wazuh SIEM security automation

## Sample Output
The AI analyzer produces detailed security reports like this:

- **Alert:** Windows application crash
- **MITRE ATT&CK:** T1499 (Endpoint Denial of Service)
- **Risk Score:** 75/100
- **Action:** Investigate immediately

## Results
- 25 alerts analyzed automatically
- 8 High severity threats detected
- 6 Medium severity threats detected
- Full JSON report generated

## Architecture
Windows Agent → Wazuh Manager (Kali Linux) → OpenSearch → Python Script → OpenAI GPT → JSON Report

## Screenshots

### File Integrity Monitoring
![File Integrity Monitoring](<img width="956" height="533" alt="File Integrity Monitoring" src="https://github.com/user-attachments/assets/83196068-8944-4f8e-a836-d2e2cd20e030" />

### Malware Detection
![Malware Detection](<img width="956" height="536" alt="Malware Detection" src="https://github.com/user-attachments/assets/7891c410-5172-4f67-b5e3-81783f8ba95c" /> 
### MITRE ATT&CK Events
![MITRE ATT&CK Events](<img width="958" height="533" alt="MITRE ATT CK Events" src="https://github.com/user-attachments/assets/ea9799a3-cc74-4b65-94b6-8f221de1e1f0" />

### MITRE ATT&CK Framework
![MITRE ATT&CK Framework](<img width="956" height="506" alt="MITRE ATT CK Framework" src="https://github.com/user-attachments/assets/8b632224-f202-40e8-b034-e66914f8374e" />


### Threat Hunting Events
![Threat Hunting](<img width="951" height="317" alt="wazuh_threat_hunting_alerts" src="https://github.com/user-attachments/assets/5673c088-9eb6-4649-8666-a5f36d1b646a" />

### Sigma Rules Backend
![Sigma Rules](<img width="953" height="379" alt="sigma rule " src="https://github.com/user-attachments/assets/d5cdd7ad-47c8-4738-bf00-30528fce13a7" />

### OpenSearch Security
![OpenSearch](<img width="929" height="193" alt="WazuhOpenSearch" src="https://github.com/user-attachments/assets/f99fdfc1-7c01-4c24-9398-6b4616c61476" />

### OpenSearch Security
<img width="929" height="193" alt="Wazuh OpenSearch" src="https://github.com/user-attachments/assets/f99fdfc1-7c01-4c24-9398-6b4616c61476" />

### Python Automation Script (wazuh-AI-agent.py)
<img width="959" height="538" alt="wazuh-AI-agent py" src="https://github.com/user-attachments/assets/765fa19b-8f6c-44f0-8776-58c8a2534c2e" />

### Successful Pipeline Connection (Terminal Output)
<img width="648" height="370" alt="Test-Connectivity" src="https://github.com/user-attachments/assets/9c5f003a-2796-40c0-8cd5-e153692b7c70" />

### Windows Services (Wazuh Agent)
<img width="957" height="539" alt="services" src="https://github.com/user-attachments/assets/2cf0463b-7b5a-4147-9972-ab9c6e306012" />

### Event Viewer
<img width="947" height="538" alt="Event Viewer" src="https://github.com/user-attachments/assets/f4c21ee5-f8d4-4de2-919c-dfe7fc6b2a4a" />

### Registry Editor
<img width="959" height="539" alt="Registry Editor" src="https://github.com/user-attachments/assets/ff27c6af-1563-499b-9d5c-908aa8474a08" />

