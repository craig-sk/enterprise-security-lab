# enterprise-security-lab
Windows Server 2016 and Kali Linux Virtual Lab This repository contains setup instructions, configurations, and screenshots for deploying a Windows Server 2016 domain controller, conducting network scans using Kali Linux (Nmap), analyzing traffic with Wireshark, and performing basic password cracking using 


Question 1: Hardware and Setup

Create a virtual lab (GNS3 or Hyper-V) with the following:

Windows Server 2016

OS: Windows Server 2016 Standard/Datacenter

IP: (Choose suitable IP)

Subnet: 255.255.240.0

Hostname: DC-SRV

Password: @dm1np@$8w0rd


Kali Linux

IP: 172.20.104.151

Subnet: 255.255.240.0



---

1.1 Promote DC-SRV as domain controller in the example.net forest. (4 Marks)

1.2 Install Wireshark. (3 Marks)

1.3 Allow inbound TCP port 22 (any remote port) through firewall. (5 Marks)

1.4 Capture and analyze network traffic in Wireshark with screenshots and conclusions. (8 Marks)


---

Question 2: Kali Linux & Packet Analysis

2.1 (Kali)

Perform Nmap scans:

Ping sweep of the network

Full scan on DC-SRV
(Leave terminal open) 


2.2 (DC-SRV)

Use Wireshark to filter for Kali Linux packets with the TCP ACK flag.
Save the filter. 

2.3 (Kali)

Use Hashcat with password_hashes.txt to crack hashes.
Submit screenshot of results. 



---

Question 3: Domain User Creation

3.1 (DC-SRV)

Create a domain user (your name) in the example.net domain with the following settings:

Must change password at next logon

Password never expires


/enterprise-pentest-lab
├── /documentation
│   ├── environment-setup.md      # Lab setup instructions
│   ├── assessment-objectives.md  # Task breakdown
│   └── findings-report.md       # Analysis conclusions
├── /screenshots
│   ├── wireshark/               # Packet captures
│   ├── nmap/                    # Scan results
│   └── hashcat/                 # Password cracking proofs
├── /scripts (optional)
│   ├── nmap_scan.sh             # Automated scan script
│   └── firewall_rules.ps1       # Windows firewall config
└── README.md                    # Project overview
