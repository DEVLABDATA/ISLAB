# ISLAB

# 🔐 Cyber Security Lab Experiments

This repository contains the commands and basic execution steps used for Cyber Security Laboratory experiments performed using Kali Linux, Docker, Nessus, MobSF, OWASP ZAP, and Digital Forensics tools.

---

 1

## Commands Used

```bash
ip a
```

```bash
nmap -sn <network-range>
```

```bash
nmap -sS <target-ip>
```



3 

## Install Docker

```bash
sudo apt update
```

```bash
sudo apt install docker.io -y
```

## Start Docker

```bash
sudo systemctl start docker
```

## Download MobSF

```bash
sudo docker pull opensecurity/mobile-security-framework-mobsf:latest
```

## Run MobSF

```bash
sudo docker run -it -p 8000:8000 opensecurity/mobile-security-framework-mobsf
```

## Check Running Containers

```bash
sudo docker ps
```

## Stop Running Containers

```bash
sudo docker stop $(docker ps -q)

```

---

 4 

## Go to Downloads Folder
```bash
https://www.tenable.com/downloads/nessus?utm_source=chatgpt.com&loginAttempted=true
```

```bash
cd ~/Downloads
```

## Install Nessus

```bash
sudo dpkg -i Nessus*.deb
```

## Fix Dependency Errors

```bash
sudo apt -f install -y
```

## Start Nessus

```bash
sudo systemctl start nessusd
```

## Stop Nessus

```bash
sudo systemctl stop nessusd
```

## Check Nessus Status

```bash
sudo systemctl status nessusd
```

---

 5 

## Menu Navigation

```bash
https://www.exterro.com/digital-forensics-software/ftk-imager?utm_source=chatgpt.com
```
```text
File → Create Disk Image
```

```text
Select Source → Logical Drive
```

```text
Select Image Type → Raw (dd)
```

---

6 

## Steps
```bash
https://download.cnet.com/saft/3000-2653_4-75878117.html
```

```text
Connect Android Device
```

```text
Enable USB Debugging
```

```text
Extract Call Logs / SMS / Contacts
```

---

7 

## Install OWASP ZAP

```bash
sudo apt update
```

```bash
sudo apt install zaproxy -y
```

## Run ZAP

```bash
zaproxy
```

## Scanning Options

```text
Analyze → Spider
```
```bash
http://demo.testfire.net
```
```text
Analyze → Active Scan
```
# 8 

## Update System

```bash
sudo apt update && sudo apt upgrade -y
```

---

## Install Required Packages

```bash
sudo apt install iptables squid -y
```

---

## Check Existing Firewall Rules

```bash
sudo iptables -L
```

---

## Block HTTPS Traffic (Port 443)

```bash
sudo iptables -A INPUT -p tcp --dport 443 -j DROP
```

---

## Block Specific IP Address

```bash
sudo iptables -A INPUT -s 192.168.1.10 -j DROP
```

---

## Allow SSH Traffic

```bash
sudo iptables -A INPUT -p tcp --dport 22 -j ACCEPT
```

---

## Start Squid Service

```bash
sudo systemctl start squid
```

---

## Enable Squid Service

```bash
sudo systemctl enable squid
```

---

## Check Squid Status

```bash
sudo systemctl status squid
```

---

# 🔹 Tools Used

- Kali Linux
- iptables
- Squid

---

# 🛠️ Tools Used

- Kali Linux
- Nmap
- Docker
- MobSF
- Nessus
- OWASP ZAP
- FTK Imager
- SAFT

---

# 📌 Notes

- Use only authorized systems and test environments.
- Some experiments require internet access.
- MobSF requires Docker to be running.
- Nessus uses port `8834`.
- OWASP ZAP is used only for educational/testing purposes.

---

# 👨‍💻 Author

Cyber Security Lab Experiments Repository
