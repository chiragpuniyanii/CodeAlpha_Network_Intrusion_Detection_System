# Network Intrusion Detection System (NIDS) using Snort and Suricata

## Overview
This project implements a Network Intrusion Detection System (NIDS) using Snort and Suricata, with log visualization through the ELK stack.

---

## **Installation Steps**
### 1. Set Up Environment
```bash
sudo apt update && sudo apt upgrade -y
```

### 2. Install Snort
```bash
sudo apt install snort -y
```
Edit `/etc/snort/snort.conf` and add rules in `/etc/snort/rules/local.rules`.

### 3. Install Suricata
```bash
sudo apt install suricata -y
```
Edit `/etc/suricata/suricata.yaml` and add rules in `/etc/suricata/rules/local.rules`.

### 4. Install ELK Stack
```bash
sudo apt install elasticsearch logstash kibana -y
```
Start services and access Kibana at `http://localhost:5601`.

---

## **Testing**
Send ICMP packets using `ping` and monitor logs in Snort/Suricata.

---

## **Project Structure**
- `snort.conf` - Snort Configuration
- `suricata.yaml` - Suricata Configuration
- `local.rules` - Custom NIDS Rules

---

## **Contributors**
- Chirag Puniyani ([GitHub](https://github.com/chiragpuniyanii))

---

## **License**
This project is licensed under the MIT License.

---

*Happy Securing!* 🚀

