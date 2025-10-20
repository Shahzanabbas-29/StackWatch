<div align="center">

# 🖥️ StackWatch

### Real-Time Server Monitoring Dashboard

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://streamlit.io/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Maintenance](https://img.shields.io/badge/Maintained-Yes-brightgreen?style=for-the-badge)](https://github.com/Shahzanabbas-29/StackWatch)

*Monitor your infrastructure with style and precision*

![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=22&pause=1000&color=FF4B4B&center=true&vCenter=true&width=600&lines=Real-Time+Server+Monitoring;Cross-Platform+Support;Beautiful+UI+Dashboard;SSH+Secure+Connections)

[Features](#-features) • [Installation](#-installation) • [Usage](#️-usage) • [Security](#️-security) • [Documentation](#-documentation)

---

</div>

## 📖 Overview

**StackWatch** is a powerful, lightweight server monitoring solution built with Streamlit. Connect to remote servers via SSH and monitor critical metrics in real-time through an elegant, interactive dashboard.

Perfect for DevOps teams, system administrators, and anyone managing multiple server infrastructures.

<!-- Add a demo GIF here when available -->
<!-- ![Demo](demo.gif) -->



<br>

## ✨ Features

<div align="center">

```mermaid
graph LR
    A[🖥️ Servers] -->|SSH| B[StackWatch]
    B --> C[📊 CPU Metrics]
    B --> D[💾 Memory Stats]
    B --> E[📂 Disk Usage]
    B --> F[🔄 Real-Time Updates]
    style B fill:#FF4B4B,stroke:#333,stroke-width:4px,color:#fff
```

</div>

<table>
<tr>
<td width="50%">

### 🔄 Real-Time Updates
Automatic refresh every 30 seconds ensures you're always viewing the latest metrics without manual intervention.

</td>
<td width="50%">

### 📊 Comprehensive Metrics
Monitor CPU load, memory utilization, and filesystem usage across all your servers.

</td>
</tr>
<tr>
<td width="50%">

### 🎨 Beautiful UI
Custom-designed interface with color-coded health indicators for instant status recognition.

</td>
<td width="50%">

### 🌐 Multi-Platform
Full support for Linux, HP-UX, AIX, and SunOS operating systems.

</td>
</tr>
<tr>
<td width="50%">

### ⚡ Lightning Fast
Built with performance in mind - minimal overhead, maximum insights.

</td>
<td width="50%">

### 🔐 Secure Connections
SSH-based authentication ensures secure server communication.

</td>
</tr>
</table>

<br>

## 🛠️ Tech Stack

<div align="center">

| Component | Technology | Version |
|-----------|-----------|---------|
| **Frontend Framework** | ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white) | Latest |
| **Backend Language** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) | 3.8+ |
| **SSH Library** | ![Paramiko](https://img.shields.io/badge/Paramiko-000000?style=flat-square) | Latest |
| **Data Processing** | ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white) | Latest |
| **Auto-refresh** | ![Streamlit](https://img.shields.io/badge/streamlit--autorefresh-FF4B4B?style=flat-square) | Latest |

<img src="https://skillicons.dev/icons?i=python,linux,git,github,vscode" />

</div>

<br>

## 🚀 Installation

<div align="center">

```mermaid
graph TD
    A[📥 Clone Repository] --> B[🐍 Create Virtual Environment]
    B --> C[📦 Install Dependencies]
    C --> D[⚙️ Configure Servers]
    D --> E[🚀 Launch StackWatch]
    E --> F[🎉 Start Monitoring!]
    style A fill:#4CAF50,stroke:#333,stroke-width:2px,color:#fff
    style F fill:#FF4B4B,stroke:#333,stroke-width:2px,color:#fff
```

</div>

### Prerequisites

- Python 3.8 or higher
- SSH access to target servers
- Basic understanding of server monitoring

### Quick Start

1️⃣ **Clone the Repository**

```bash
git clone https://github.com/Shahzanabbas-29/StackWatch.git
cd StackWatch
```

2️⃣ **Create Virtual Environment** (Recommended)

```bash
# Linux/MacOS
python -m venv venv
source venv/bin/activate

# Windows
python -m venv venv
venv\Scripts\activate
```

3️⃣ **Install Dependencies**

```bash
pip install -r requirements.txt
```

4️⃣ **Configure Your Servers**

Add your server credentials to `.streamlit/secrets.toml` (see [Security](#️-security) section):

```toml
[servers]
hosts = ["192.168.1.10", "192.168.1.11"]
users = ["monitor", "admin"]
# Use SSH keys instead of passwords in production!
```

5️⃣ **Launch StackWatch**

```bash
streamlit run app.py
```

6️⃣ **Open Your Browser**

Navigate to `http://localhost:8501` and start monitoring!

<div align="center">

![Installation](https://img.shields.io/badge/Installation-Easy-brightgreen?style=for-the-badge&logo=checkmarx&logoColor=white)
![Setup Time](https://img.shields.io/badge/Setup_Time-5_Minutes-blue?style=for-the-badge&logo=clockify&logoColor=white)

</div>

<br>

## 🗂️ Project Structure

```
StackWatch/
│
├── 📄 app.py                    # Main Streamlit application
├── 📋 requirements.txt          # Python dependencies
├── 🖼️ SAIL_Logo.png            # Dashboard logo
│
├── 📁 .streamlit/
│   └── secrets.toml             # Secure credentials (DO NOT COMMIT)
│
├── 📁 utils/                    # (Optional) Helper modules
│   ├── ssh_manager.py           # SSH connection handling
│   └── metrics_parser.py        # Metric extraction utilities
│
└── 📄 README.md                 # You are here!
```

<br>

## ⚙️ Usage

### Dashboard Overview

Once launched, StackWatch displays:

<div align="center">

```mermaid
pie title Server Metrics Distribution
    "CPU Usage" : 30
    "Memory Usage" : 40
    "Disk Usage" : 30
```

</div>

<table>
<tr>
<td width="25%" align="center">
<h4>🎯 Server Status</h4>
Real-time UP/DOWN indicators
</td>
<td width="25%" align="center">
<h4>⚙️ CPU Metrics</h4>
Current load percentages
</td>
<td width="25%" align="center">
<h4>💾 Memory Stats</h4>
Used vs. available memory
</td>
<td width="25%" align="center">
<h4>📂 Disk Usage</h4>
Filesystem utilization alerts
</td>
</tr>
</table>

### Example Output

```
┌─────────────────────────────────────────────────────────────┐
│ 🖥️  Server: 10.145.25.5                   Status: 🟢 UP    │
├─────────────────────────────────────────────────────────────┤
│ ⚙️  CPU Usage: 35.4%                                        │
│ 💾 Memory Usage: 2048MB / 4096MB (50%)                     │
│                                                             │
│ 📂 Filesystem Utilization:                                 │
│ ┌───────────┬──────┬──────┬───────┬──────┬─────────────┐ │
│ │ Filesystem│ Size │ Used │ Avail │ Use% │ Mounted on  │ │
│ ├───────────┼──────┼──────┼───────┼──────┼─────────────┤ │
│ │ /dev/sda1 │  20G │  15G │   5G  │  75% │ /           │ │
│ │ tmpfs     │  1G  │ 0.1G │  0.9G │  10% │ /tmp        │ │
│ └───────────┴──────┴──────┴───────┴──────┴─────────────┘ │
└─────────────────────────────────────────────────────────────┘
```

### Health Indicators

<div align="center">

| Indicator | Status | CPU Range | Action Required |
|-----------|--------|-----------|-----------------|
| 🟢 Green | Healthy | 0-60% | None |
| 🟡 Yellow | Warning | 61-85% | Monitor closely |
| 🔴 Red | Critical | 86-100% | Immediate attention |
| ⚫ Gray | Offline | N/A | Check connectivity |

![Status](https://img.shields.io/badge/Status-Monitoring-brightgreen?style=for-the-badge&logo=statuspage&logoColor=white)
![Uptime](https://img.shields.io/badge/Uptime-99.9%25-success?style=for-the-badge&logo=apache&logoColor=white)

</div>

<br>

## 🛡️ Security

> **⚠️ CRITICAL: This section must be read before deployment**

<div align="center">

```mermaid
sequenceDiagram
    participant User
    participant StackWatch
    participant SSH
    participant Server
    User->>StackWatch: Request Metrics
    StackWatch->>SSH: Establish Secure Connection
    SSH->>Server: Authenticate with Key
    Server->>SSH: Return Metrics
    SSH->>StackWatch: Encrypted Data
    StackWatch->>User: Display Dashboard
```

</div>

### 🚨 Security Checklist

- [ ] **NEVER commit credentials** to version control
- [ ] Use `.streamlit/secrets.toml` or environment variables
- [ ] Implement SSH key authentication (not passwords)
- [ ] Use strict host key verification in production
- [ ] Rotate all credentials immediately if exposed
- [ ] Enable firewall rules for SSH access
- [ ] Implement rate limiting for dashboard access
- [ ] Use HTTPS in production environments

### Secure Credential Management

**❌ DON'T DO THIS:**
```python
# NEVER hardcode credentials
username = "admin"
password = "password123"  # TERRIBLE IDEA
```

**✅ DO THIS INSTEAD:**

Create `.streamlit/secrets.toml`:
```toml
[ssh]
host = "192.168.1.10"
username = "monitor"
key_path = "/home/user/.ssh/id_rsa"
```

Access in code:
```python
import streamlit as st

host = st.secrets["ssh"]["host"]
username = st.secrets["ssh"]["username"]
key_path = st.secrets["ssh"]["key_path"]
```

### SSH Key Authentication

Replace password authentication with SSH keys:

```bash
# Generate SSH key pair
ssh-keygen -t ed25519 -C "stackwatch@monitoring"

# Copy public key to server
ssh-copy-id -i ~/.ssh/id_ed25519.pub user@server
```

### If Credentials Were Exposed

<div align="center">

```mermaid
graph TD
    A[🚨 Credentials Exposed] --> B[🔄 Rotate ALL Credentials]
    B --> C[🔑 Revoke API Keys]
    C --> D[📋 Review Access Logs]
    D --> E[🧹 Clean Git History]
    E --> F[🔐 Enable 2FA]
    style A fill:#ff4444,stroke:#333,stroke-width:3px,color:#fff
    style F fill:#44ff44,stroke:#333,stroke-width:3px,color:#000
```

</div>

1. **Rotate ALL credentials immediately**
2. **Revoke compromised API keys**
3. **Review access logs for suspicious activity**
4. **Clean git history** (use `git-filter-repo`)
5. **Enable 2FA where available**

<br>

## 🎯 Roadmap

### 🔜 Coming Soon

- [ ] 🔑 SSH key authentication (priority)
- [ ] 📧 Email/SMS alerts for critical thresholds
- [ ] 📊 Historical data graphing and trends
- [ ] 🐳 Docker containerization
- [ ] 🔐 Built-in authentication system
- [ ] 🌙 Dark mode toggle

### 💡 Future Ideas

- [ ] Multi-tenant support
- [ ] Custom alert rules engine
- [ ] Integration with Prometheus/Grafana
- [ ] Mobile-responsive design
- [ ] Database connection monitoring
- [ ] Kubernetes cluster monitoring
- [ ] Export reports to PDF/CSV

<br>

## 🤝 Contributing

<div align="center">

![Contributors](https://img.shields.io/github/contributors/Shahzanabbas-29/StackWatch?style=for-the-badge&color=FF4B4B)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=for-the-badge)
![Code Size](https://img.shields.io/github/languages/code-size/Shahzanabbas-29/StackWatch?style=for-the-badge)

</div>

Contributions are welcome! Here's how you can help:

```mermaid
graph LR
    A[🍴 Fork] --> B[🔧 Branch]
    B --> C[💾 Commit]
    C --> D[📤 Push]
    D --> E[🎉 PR]
    style A fill:#4CAF50,stroke:#333,stroke-width:2px
    style E fill:#FF4B4B,stroke:#333,stroke-width:2px
```

1. 🍴 Fork the repository
2. 🔧 Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. 💾 Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. 📤 Push to the branch (`git push origin feature/AmazingFeature`)
5. 🎉 Open a Pull Request

Please read our [Contributing Guidelines](CONTRIBUTING.md) for details.

<br>

## 📚 Documentation

For detailed documentation, visit our [Wiki](https://github.com/Shahzanabbas-29/StackWatch/wiki) or check out:

- [Configuration Guide](docs/configuration.md)
- [Troubleshooting](docs/troubleshooting.md)
- [API Reference](docs/api.md)
- [Best Practices](docs/best-practices.md)

<br>

## 🐛 Known Issues

- Auto-refresh may cause session state issues with large server counts
- Some AIX systems require custom command formatting
- Windows SSH client compatibility limitations

See [Issues](https://github.com/Shahzanabbas-29/StackWatch/issues) for full list.

<br>

## 📊 Stats

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api/pin/?username=Shahzanabbas-29&repo=StackWatch&theme=radical)

![Language Stats](https://github-readme-stats.vercel.app/api/top-langs/?username=Shahzanabbas-29&layout=compact&theme=radical)

</div>

<br>

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

<div align="center">

```
MIT License - Copyright (c) 2024 Shahzan Abbas
Free to use, modify, and distribute with attribution.
```

![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge&logo=opensourceinitiative&logoColor=white)

</div>

<br>

## 👨‍💻 Author

<div align="center">

### Shahzan Abbas

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Shahzanabbas-29)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:shahzanabbas@example.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/shahzanabbas)

![Profile Views](https://komarev.com/ghpvc/?username=Shahzanabbas-29&color=FF4B4B&style=for-the-badge)

</div>

<br>

## 🙏 Acknowledgments

- Built with [Streamlit](https://streamlit.io/)
- SSH connectivity via [Paramiko](https://www.paramiko.org/)
- Icons from [Lucide](https://lucide.dev/)
- Inspired by modern DevOps practices

<br>

## ⭐ Show Your Support

If you found this project helpful, please give it a ⭐ on GitHub!

<div align="center">

[![Star History Chart](https://api.star-history.com/svg?repos=Shahzanabbas-29/StackWatch&type=Date)](https://star-history.com/#Shahzanabbas-29/StackWatch&Date)

[![GitHub Stars](https://img.shields.io/github/stars/Shahzanabbas-29/StackWatch?style=social)](https://github.com/Shahzanabbas-29/StackWatch/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/Shahzanabbas-29/StackWatch?style=social)](https://github.com/Shahzanabbas-29/StackWatch/network/members)
[![GitHub Watchers](https://img.shields.io/github/watchers/Shahzanabbas-29/StackWatch?style=social)](https://github.com/Shahzanabbas-29/StackWatch/watchers)

---

<sub>Built with ❤️ by developers, for developers</sub>

![Wave](https://raw.githubusercontent.com/mayhemantt/mayhemantt/Update/svg/Bottom.svg)

**[⬆ Back to Top](#-stackwatch)**

</div>

---

### ⚠️ Disclaimer

This tool is intended for **internal monitoring purposes only**. Do not use or share production credentials publicly or in any version-controlled repository. Always follow your organization's security policies and best practices.

<div align="center">

![Made with Love](https://img.shields.io/badge/Made%20with-❤️-red?style=for-the-badge)
![Powered by Coffee](https://img.shields.io/badge/Powered%20by-☕-brown?style=for-the-badge)

</div>

