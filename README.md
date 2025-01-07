## Objective

To effectively install, configure, and utilize Snort as an Intrusion Detection System (IDS) on Ubuntu 22.04 LTS, including setting up custom and community based rules, verifying installation, and managing rule paths.

### Skills Learned

- Installation and Configuration
  - Installing Snort 3 on Ubuntu 22.04 LTS.
  - Updating shared libraries and installing prerequisites such as hyperscan.
  - Troubleshooting of installation, setup and configuration issues.

- Rule Management
  - Creating and managing custom rules for detecting specific network traffic.
  - Modifying configuration files to include and manage rule sets and paths.
  - Obtaining and integrating Oink codes for accessing additional rules.

- Service Management
  - Enabling and starting the Snort IDS service using system commands.
  - Configuring network adapter settings in Snort’s configuration file.

- Verification and Testing
  - Running Snort to monitor network traffic and confirm rule functionality.
  - Using command-line tools to filter and detect specific network traffic.

- Configuration Management
  - Modifying Snort configuration files to integrate pulledpork’s or community based rules.
  - Ensuring proper settings and paths for rule management.

### Tools Used

- Snort3. Open-source IDS/IPS tool for network traffic analysis.
- Hyperscan. Prerequisite for Snort 3 installation.
- Oinkcode. Access code for Snort rules.
- PulledPork. Tool for managing Snort rules.

## Lab Information

<p align="center">
<img src="https://imgur.com/8rTkja3.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>Network Diagram</b>
<br/>

### Lab Hosts

- FortiGate NGFW Eval
  - Router and Firewall.
- Ubuntu 22.04 LTS
  - Snort as an IDS.
- Ubuntu 22.04 LTS          
  - SSH server.
- Attacker's machine
  - Perform ICMP, SSH Authentication and nmap.

- Checking network connectivty on hosts
<p align="center">
<img src="https://imgur.com/xPpyFIL.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<p align="center">
<img src="https://imgur.com/mO0xUSv.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>Fortigate NGFW status.</b>
<br/>

<p align="center">
<img src="https://imgur.com/TAgKfKr.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/74boOf5.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>Snort IDS IP address and status.</b>
<br/>

<p align="center">
<img src="https://imgur.com/ZxKW86Y.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>Ubuntu server IP address and status.</b>
<br/>

- Generate traffic
<p align="center">
<img src="https://imgur.com/tjUO2Li.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>Perform ICMP and SSH Attempt to SSH Server.</b>
<br/>

<p align="center">
<img src="https://imgur.com/pGPv4S8.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>Attacker's machine perform nmap to SSH server.</b>
<br/>

 - Server alert
<p align="center">
<img src="https://imgur.com/t1qHDYN.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>ICMP and SSH Authentication custom alert.</b>
<br/>

<p align="center">
<img src="https://imgur.com/8IJXuEP.png" height="40%" width="40%" alt="Device Specification"/>
<br/>
<b>Using the pulledpork.rules to alert nmap attempt.</b>
<br/>

## Outcome

- Created and implemented custom and community based Snort rules to detect network threats.
- Managed and updated Snort configurations and rule paths effectively.
- Verified Snort’s functionality and performance in a virtual environment.
- Utilized command-line tools to filter and detect network traffic.
- Alerts were triggered by the ICMP traffic, SSH authentication attempts, and nmap scans.

## Acknowledgements
- [Snort](https://docs.snort.org/)
- Installation guide from [MyDFIR](https://github.com/MyDFIR/snort3-install-guide)

## Disclaimer

This portfolio is intended for educational and ethical cybersecurity research purposes only. All projects were conducted in a controlled, personal laboratory environment. The author(s) strongly condemn any illegal or unethical use of the information or code presented here. Unauthorized access to any system is strictly forbidden. The author(s) assume no responsibility for any actions taken by third parties using this information.
