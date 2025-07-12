# 🛠️ Auto-Healer Linux

A lightweight, self-healing automation tool designed to monitor and restart critical Linux services in real-time using Bash scripting. This project ensures high availability by reducing downtime and manual intervention for system administrators.

---

## 📌 Project Overview

**Auto-Healer Linux** is a simple yet powerful tool written in Bash to monitor essential system services like `apache2`, `ssh`, and `cron`. If any of these services fail, the tool automatically restarts them, logs the incident, and optionally sends an email notification to the system administrator. This project is ideal for academic use, small-scale server setups, and self-hosted systems.

---

## 📋 Features

- 🟢 Monitors system services continuously
- 🔄 Automatically restarts failed services
- 📧 Sends email notifications on service failure/restart
- 📓 Logs all events and actions
- 🕑 Runs periodically using `cron`
- 🌐 Optional GUI/web interface with Flask + HTML/CSS/JS

---

## 🔍 Problem Statement

In typical Linux environments, the failure of core services (e.g., web servers, SSH, cron jobs) can lead to major disruptions. Traditional monitoring requires manual checking and restarting, which is time-consuming and error-prone. Auto-Healer Linux solves this by automating service monitoring and recovery.

---

## 🎯 Objectives

- Monitor essential Linux services using `systemctl`.
- Auto-restart inactive or failed services.
- Log all actions (failures, restarts) to a custom log file and system log.
- Send alert emails to system administrators.
- Schedule script execution using `cron`.

---

## 🧰 Tools & Technologies

| Component   | Technology                |
|-------------|----------------------------|
| Language    | Bash                       |
| Scheduler   | cron                       |
| Monitoring  | systemctl, logger          |
| Notification| mail / mailx               |
| Platform    | Kali Linux (or any Linux)  |
| Web UI (optional) | Python Flask, HTML, CSS, JS |

---

## 🖥️ Installation & Usage

### 1. Clone this Repository

```bash
git clone https://github.com/your-username/auto-healer-linux.git
cd auto-healer-linux

2. Make the Script Executable
bash
Copy
Edit
chmod +x auto-healer.sh

3. Install Required Packages
bash
Copy
Edit
sudo apt-get install mailutils

4. Run the Script Manually (Optional)
bash
Copy
Edit
./auto-healer.sh

5. Schedule with Cron (every 5 minutes)
bash
Copy
Edit
crontab -e
# Add this line
*/5 * * * * /path/to/auto-healer.sh

🧪 Output
✅ Terminal output showing monitored and restarted services
📄 /var/log/autohealer.log contains timestamped logs
📧 Email alerts sent on service failure

GUI
https://singular-mooncake-0db712.netlify.app/
Entering service name
Buttons to check status, restart service, show logs
Live log stream area
Built using HTML, CSS, JavaScript (Fetch API)

📈 Future Scope
Add uptime tracking and analytics
Telegram/Slack notifications
Use Python for enhanced error handling
Deploy multi-node or distributed monitoring

📚 Deliverables
Bash script: auto-healer.sh
Cron job setup instructions
Log files
Sample email notification
Project report & presentation
Flask web interface (optional)

🤝 Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

📄 License
This project is open-source and free to use under the MIT License.

🙏 Acknowledgements
Developed under the guidance of Shashidhar
Part of Cyber Security Minor Project at TEKS Academy

📞 Contact
P. Rakesh
📱 +91 9515924411
📧 your-email@example.com
📍 India
