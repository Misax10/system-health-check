## 🖥️ System Health Check Script for IT Support | Bash Script for macOS

A professional, automated Bash script that collects key system diagnostics and generates a detailed health report — tailored for IT Support environments.

---

✅ Features:
- Collects disk, memory, CPU, and uptime data
- Displays top 5 active processes
- Flags system alerts (e.g., low memory, high disk usage)
- Saves a time-stamped log to the `logs/` folder
- Automatically sends the report via email (if mail is available)
- Supports automation with `cron` for daily/weekly scheduling

📄 Includes:
- Sample report as PDF in `demo/`
- Easy-to-read, professional logs
- Optional screenshots and full walkthrough

🧰 Built For:
- IT Support Specialists
- Sysadmin trainees
- Students preparing for CompTIA A+ or real-world IT troubleshooting

📍 Works on: macOS (tested) and most Linux distros

---


## 📂 Project Structure
```
system-health-check/
├── README.md
├── health_check.sh # Main Bash script
├── logs/
│   └── example-output.txt
├── demo/
│   └── sample-report.pdf
```

## 🚀 How to Run

You can run this script manually or set it to run automatically every day.

📄 View the [Crontab Setup](crontab-setup.md)
### 🔹 Manual Run
```bash
chmod +x health_check.sh
./health_check.sh
```
## 🧰 Tools Used
- Bash (macOS/Linux)
- vm_stat, df, uptime, ps, ls, system_profiler

---
## 📸  Demo
You can view a sample system health report generated by the script here:
📄 [View Sample Report (PDF)](demo/sample-report.pdf)

---

## 📬 Contact

**Khoa Diep**  
Email: [khoadiep99@gmail.com](mailto:khoadiep99@gmail.com)  
LinkedIn: [linkedin.com/in/khoadiep](https://www.linkedin.com/in/khoadiep)

---

© 2025 Khoa Diep. All rights reserved.
