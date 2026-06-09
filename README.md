## 🏗️ Phase 1: Infrastructure & Virtualization Setup
* Hypervisor Deployment: Provisioned and configured a local virtualization environment on a physical macOS client to run a nested enterprise lab.

* Operating System Provisioning: Deployed and initialized a virtual machine running Windows Server 2022, designating it as the primary infrastructure node (DC-01).

* Virtual Networking: Configured isolated internal virtual network adapters to establish a controlled environment for safe security testing and identity management simulations.

## 🔑 Phase 2: Active Directory Domain Services & Automation
Domain Promotion: Configured and promoted the server to a root Domain Controller, establishing the local enterprise directory forest (plushrealty.local).

* Logical Organization: Built a scalable Organizational Unit (OU) hierarchy to separate corporate headquarters (PRG-HQ), regional branches (PRG-Branches), and external contractors (PRG-External).

* CLI Account Automation: Engineered and executed command-line scripts to rapidly provision 7 distinct employee user profiles into the directory database, standardizing logon naming conventions and initial credential baselines.

## 🛡️ Phase 3: Advanced Group Policy Hardening (GPOs)
Custom Security Object Baseline: Isolated custom domain rules from default system templates by engineering a dedicated Group Policy Object (PRG-Security-Policy) linked directly to the root domain.

* Granular Password Lifecycle Control: Enforced strict corporate credential safety windows by establishing a 90-day maximum password age (forcing rotation) and a 30-day minimum password age (preventing rapid reuse back-to-back), paired with a 12-character minimum length and complexity mandate.

* Brute-Force Lockout Defense: Mitigated credential-stuffing and brute-force risks by configuring an Account Lockout Threshold of 5 invalid logon attempts, successfully forcing updates live via command-line updates (gpupdate /force).

* Desktop & Control Panel Lockdown: Hardened user desktop environments across the enterprise by pushing domain-wide restrictions that blocked access to the Windows Control Panel/Settings app and enforced a standardized corporate desktop wallpaper.

## 📁 Phase 4: Enterprise File Services & NTFS Security
Shared Infrastructure: Built and provisioned a central network repository by creating a shared corporate directory (PRG folder).

* Role-Based Privilege Lockout: Configured explicit NTFS permissions and network share folder settings to host enterprise assets, securing an Employee_Handbook.txt file by explicitly locking it down as Read-Only for standard users to protect regulatory data from alteration.

## 🖥️ Phase 5: Remote Access & Support Engineering
Enterprise Client Deployment: Deployed TeamViewer as a third-party remote management solution to simulate a modern, cloud-brokered help desk support model.

* Cross-Platform Engineering: Established a secure remote pipeline bridging the physical macOS architecture (Client) to the virtualized Windows Server environment (Host).

* Unattended Access Validation: Configured automated startup services and permanent host credentials to support administrative maintenance without manual console intervention.

* System Architecture Documentation: Drafted and verified accurate technical documentation directly inside the remote host session to correctly define client-host relationships according to industry standards.

## 🚀 Key Skills Demonstrated
* Systems Administration | Virtualization (macOS/Windows Server) | Active Directory Domain Services (AD DS) | Identity & Access Management (IAM) | PowerShell & CLI Automation | Group Policy Management (GPOs) | Cybersecurity Hardening & Environment Lockdown | NTFS Permissions & File Share Security | Enterprise Remote Support Tools (TeamViewer)

<!--
**jrmsy19-glitch/jrmsy19-glitch** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
