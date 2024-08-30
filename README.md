# 🚀 Active Directory Lab Project


**Welcome to the AD Lab Playground!**  
Building an enterprise-grade environment using:
- 🖥️ **Windows 10** (Client)
- 🐉 **Kali Linux** (PenTest)
- 📊 **Splunk Server** (Log Ninja)
- 🛡️ **Windows Server 2022** (AD Controller)

## ⚙️ Lab Setup

### 🔧 Domain Controller (Windows Server 2022)
- Install **AD DS** and promote the server:
  - `Add-WindowsFeature -Name AD-Domain-Services -IncludeManagementTools`
  - **Promote to DC**: `Install-ADDSForest -DomainName "yourdomain.com"`
- Configure DNS & Group Policy

### 🖥️ Windows 10 Client
- **Join Domain**:
  - `Settings > Accounts > Access work or school > Connect`
- Setup user profiles & Group Policies

### 🐉 Kali Linux (Hacker’s Playground)
- Network config:
  - `nano /etc/network/interfaces`
  - `ifconfig eth0 up`
- Install tools like `nmap`, `Metasploit`

### 📊 Ubuntu Server (Splunk) Version 22.04
- [Download URL](https://ubuntu.com/download/alternative-downloads)
- **Install Splunk**: `dpkg -i splunk-package.deb`
  ```bash
  sudo apt-get update && sudo apt-get upgrade -y
- Set up log forwarding (WEF):
  - `wevtutil qe Security /c:5 /rd:true /f:text`
  - Forward logs from Windows/Linux to Splunk

## 🌟 Features Coming Soon
- 💻 **SIEM Integration**: Level up Splunk as your SIEM warrior.
- 🛡️ **IDS Setup**: Deploy **Snort** or **Suricata**.
- 🔄 **Automation Scripts**: Get lazy with PowerShell/Bash.
- 🛠️ **Security Hardening**: Bulletproof your setup.

## 📸 Screenshots (Soon)


## 🛠️ Troubleshooting
- **Common Issue**: Connection drop?  
  **Fix**: Check `firewall rules` & DNS settings.

## 📚 Resources
- [Microsoft AD Docs](https://docs.microsoft.com/windows-server/identity/active-directory-domain-services)
- [Splunk Docs](https://docs.splunk.com/Documentation/Splunk/latest/User/WelcometotheSplunkUserDocumentation)
- [Kali Linux Docs](https://www.kali.org/docs/)

## 🛡️ Contribute
PRs & issues welcome! Let’s make this lab epic. 🎉

## 📜 License
[MIT License](LICENSE)
