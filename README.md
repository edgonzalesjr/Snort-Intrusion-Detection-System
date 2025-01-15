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
- Zenmap. The official Nmap security scanner GUI.

## Lab Information

<p align="center">
<img src="https://imgur.com/8rTkja3.png" height="50%" width="50%" alt="Device Specification"/>
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
  - Perform ping, SSH authentication and Zenmap.

## Practical Exercises

<p align="center">
<img src="https://imgur.com/xPpyFIL.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/mO0xUSv.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Fortigate NGFW status.</b>
<br/>

<p align="center">
<img src="https://imgur.com/TAgKfKr.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/74boOf5.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Snort IDS IP address and status.</b>
<br/>

<p align="center">
<img src="https://imgur.com/ZxKW86Y.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>SSH server IP address and status.</b>
<br/>

- Generate traffic
<p align="center">
<img src="https://imgur.com/tjUO2Li.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/pGPv4S8.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Attacker's machine perform ping, Zenmap and SSH authentication attempts to SSH server.</b>
<br/>

- Server alert
<p align="center">
<img src="https://imgur.com/t1qHDYN.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Ping and SSH Authentication custom alert.</b>
<br/>

<p align="center">
<img src="https://imgur.com/8IJXuEP.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Using the pulledpork.rules to alert nmap attempt.</b>
<br/>

## Outcome

- Created and implemented custom and community based Snort rules to detect network threats.
- Managed and updated Snort configurations and rule paths effectively.
- Verified Snort’s functionality and performance in a virtual environment.
- Utilized command-line tools to filter and detect network traffic.
- Alerts were triggered by the Ping traffic, SSH authentication attempts, and Zenmap scans.

## Acknowledgements

This project combines ideas and methods from various sources, such as the installation guide by MyDFIR and my personal experience. These resources provided the fundamental information and techniques, which were then modified in light of practical uses.
 - [MyDFIR](https://github.com/MyDFIR/snort3-install-guide)
 - [Snort](https://docs.snort.org/)
 - [Zenmap](https://nmap.org/zenmap/)

## Disclaimer

The projects and activities within this portfolio are for educational and ethical cybersecurity research purposes only. All work was performed in controlled environments, including isolated, personally owned laboratories, subscription-based cloud environments, and through engagement with online cybersecurity learning platforms. Any cloud-based activities and participation in online learning platforms were conducted in full compliance with their respective terms of service and acceptable use policies. These projects should not be used for any illegal or unethical activities. Unauthorized access to any computer system or network is strictly prohibited. The author(s) are not responsible for any misuse of the information or code provided.
