# scan-report
Nmap scan results and analysis for identifying open ports and potential security risks on a local network

# 1. Identify IP Configuration (Windows)
Open **Command Prompt** and run:
```cmd
ipconfig
 2. Install Nmap
Download from the official website:

👉 https://nmap.org/download.html

✔️ During installation, ensure you enable the option to add Nmap to your system PATH.
3. Scan the Network
Discover Live Hosts in the Subnet
nmap -sn 192.168.1.11
Nmap scan report for 192.168.1.00
Host is up (0.0020s latency).
4. Scan Host 192.168.1.00 for Open Ports
Full TCP Port Scan:
nmap -sS -p- 192.168.1.00

PORT     STATE SERVICE
135/tcp  open  msrpc
139/tcp  open  netbios-ssn
445/tcp  open  microsoft-ds
5357/tcp open  wsdapi

5. Packet Capture with Wireshark
📥 Install Wireshark
Download from:
👉 https://www.wireshark.org/download.html

🧪 Capture HTTP Packets
Run Wireshark as Administrator.

Select your active network interface.

Start capturing.

7. Analyze the captured HTTP traffic.
