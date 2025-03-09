Network Intrusion Detection System (NIDS) using Snort

📌 Project Overview
This project implements a Network Intrusion Detection System (NIDS) using Snort, which monitors network traffic and detects suspicious activities based on predefined rules.

🚀 Features
  Real-time network monitoring
  Detection of ICMP ping sweeps, SSH brute-force attacks, and other intrusions
  Custom Snort rule configurations
  Logging and alert generation for detected threats
  Optional visualization using ELK Stack

🛠️ Installation & Setup
1️⃣ Install Snort
On Linux (Ubuntu/Debian)
  sudo apt update && sudo apt install snort -y
On Windows
  Download and install Npcap
  Download and install Snort

2️⃣ Configure Snort Rules
Edit the Snort Rules File (/etc/snort/rules/local.rules) 

3️⃣ Run Snort to Monitor Network Traffic
Packet Logging Mode
  sudo snort -dev -i eth0 -l /var/log/snort/

4️⃣ Check Logs for Alerts
  cat /var/log/snort/alert.ids

📊 Optional: Visualizing Alerts
For better analysis, use ELK Stack (Elasticsearch, Logstash, Kibana):
  sudo apt install kibana logstash elasticsearch

📂 Project Structure
  📁 Network-Intrusion-Detection-System
  │── 📄 snort.conf           # Main Snort configuration file
  │── 📄 local.rules         # Custom Snort rules
  │── 📂 logs/               # Directory for Snort alert logs
  │── 📄 README.md           # Project documentation

📢 Contributing
Feel free to contribute by adding new detection rules, improving configurations, or optimizing log analysis!

🏆 Credits
Developed by Anant Sharma
Internship at Code Alpha

🔗 Connect with Me
💼 LinkedIn: anantsharma31
📂 GitHub: AnantCo
