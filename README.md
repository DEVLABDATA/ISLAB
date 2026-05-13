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

```text
Analyze → Active Scan
```

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
