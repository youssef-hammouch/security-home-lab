# Security Home Lab

A virtual lab to practice attack and detection.

## Goal
Attack my own machines, detect the attacks with a SIEM, and fix the weaknesses.

## Tools
VMware, OPNsense, Kali Linux, Ubuntu, Windows 7, Wazuh

## Progress

### 1. Firewall setup
OPNsense separates an "inside" and an "outside" network.

![OPNsense dashboard](Screenshots/01-opnsense-dashboard.png)
The firewall is running and managing the inside network.

![Ubuntu internet test](Screenshots/02-ubuntu-ping-internet.png)
Ubuntu reaches the internet through the firewall.
  ### 2. Outside network
Kali is on a separate outside network. A firewall rule allows it to reach the inside network.

![OPT1 firewall rule](Screenshots/03-opnsense-opt1-rule.png)

### 3. SIEM setup
Wazuh monitors the inside network.

![Wazuh dashboard](Screenshots/04-wazuh-dashboard.png)
