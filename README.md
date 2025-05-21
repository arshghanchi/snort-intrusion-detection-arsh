# Custom Snort Intrusion Detection Project

This project is a unique implementation of a network intrusion detection system using **Snort**, carried out by **Mohamed Arsh Mohamed Arif Ghanchi** as part of the **SIT327 - Network Forensics** unit at **Deakin University**. It simulates and analyzes malicious traffic to help identify potential intrusions using custom Snort rules.

## 🚀 Key Capabilities

- Detects ICMP and TCP-based network anomalies
- Custom rules for real-time traffic inspection
- Console-based alerting with log support
- Developed and tested on both Ubuntu and Windows systems
- Includes flowcharts and structured documentation

## ⚙️ Installation and Usage

### Linux (Ubuntu)

1. Install Snort:
   ```bash
   sudo apt update && sudo apt install snort
   ```

2. Configuration:
   - Set `HOME_NET` inside `/etc/snort/snort.conf`
   - Create or edit `/etc/snort/rules/local.rules`

3. Validate:
   ```bash
   sudo snort -T -c /etc/snort/snort.conf
   ```

4. Launch:
   ```bash
   sudo snort -A console -i eth0 -c /etc/snort/snort.conf
   ```

### Windows

1. Download Snort for Windows from the [official site](https://www.snort.org/downloads#windows)
2. Install [Npcap](https://npcap.com) with WinPcap compatibility enabled
3. Configure Snort with your local rules and snort.conf
4. Run:
   ```cmd
   snort.exe -A console -q -c C:\Snort\etc\snort.conf -i 1
   ```

## 🖼 Visuals

Refer to the `screenshots/` and `docs/` directories for example outputs and diagrams.

## 👤 Project Owner

- **Full Name**: Mohamed Arsh Mohamed Arif Ghanchi  
- **Student ID**: S222574204  
- **Course**: SIT327  
- **Institution**: Deakin University

## 📘 License

Distributed under the [MIT License](LICENSE). Feel free to reuse and modify with credit.
