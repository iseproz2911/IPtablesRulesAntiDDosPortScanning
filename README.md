# IPtablesRulesAntiDDosPortScanning
# WebOS Deployment on Raspberry Pi 4 with iptables Firewall Configuration

This document outlines the steps for deploying WebOS on a Raspberry Pi 4, configuring the iptables firewall, testing its resilience against common DoS/DDoS attacks, and analyzing the results.

---

## Prerequisites
- A Raspberry Pi 4 with WebOS successfully deployed.
- SSH access to the Raspberry Pi from a host machine or virtual machine.
- Required tools installed:
  - `iptables` for firewall configuration.
  - `hping3` for testing different types of attacks.

---

## Configuration Steps

### 1. Verify iptables Status
Access the Raspberry Pi via SSH and execute the following command to check the iptables status:
```bash
ssh root@<RaspberryPi_IP>
iptables -L -v -n
iptables-restore < rules.v4
```
### 2. Testing Firewall Resilience
Attack Scenarios
Perform the following attacks from a host machine or virtual machine against the WebOS on Raspberry Pi to evaluate the effectiveness of the firewall:
SYN Flood Attack
Random Source Attack
Smurf Attack
LAND Attack
PortScanning
### 3. Reporting Results
https://hackmd.io/@iamproz2911/H1vnZWmXkg
