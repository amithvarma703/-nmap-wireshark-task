# -nmap-wireshark-task
Task 1 – Local Network Port Scanning with Nmap and Wireshark
Objective:
I use Nmap to discover open ports on devices in my local network and Wireshark to analyze traffic to understand network exposure and potential vulnerabilities.

Tools Used:

Nmap (Command-line TCP SYN scan)

Wireshark (Packet capture and analysis)

Steps Taken:

Installed Nmap and Wireshark on Windows.

Identified my local IP range using ipconfig or System Information.

Performed a scan using:
nmap -sS 192.168.1.0/24 -oN scan-results.txt
Simultaneously captured traffic using Wireshark on my active network interface.

Applied the filter: tcp.flags.syn == 1 to view SYN packets used in the scan.

Analyzed responses:

SYN-ACK = port open

RST = port closed

No response = filtered.

Saved:

Nmap scan as .txt

Wireshark capture as .pcapng

Findings:

Open ports on local devices included 22 (SSH), 80 (HTTP), and 445 (SMB)

SMB service exposed = potential security risk

Recommendation: disable unused services and secure access via a  firewall

Screenshots and Files:
![Screenshot 2025-06-23 125635](https://github.com/user-attachments/assets/2eab8eae-63e4-4624-ba0b-15e29a45fd39)

![Screenshot 2025-06-23 125859](https://github.com/user-attachments/assets/19e5dd49-144d-4c4f-bea7-de41558ee907)

![Screenshot 2025-06-23 140511](https://github.com/user-attachments/assets/ab9eaeb7-cbb2-4aec-a0a2-37127c5ec47d)


thank you.
