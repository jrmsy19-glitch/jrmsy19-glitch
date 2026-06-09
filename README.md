## 🏗️ Phase 1: Infrastructure & Virtualization Setup
* Hypervisor Deployment: Provisioned and configured a local virtualization environment on a physical macOS client to run a nested enterprise lab.

* Operating System Provisioning: Deployed and initialized a virtual machine running Windows Server 2022, designating it as the primary infrastructure node (DC-01) (See Figure 1.1).

* Virtual Networking: Configured isolated internal virtual network adapters to establish a controlled environment for safe security testing and identity management simulations.

## 🔑 Phase 2: Active Directory Domain Services & Automation
Domain Promotion: Configured and promoted the server to a root Domain Controller, establishing the local enterprise directory forest (plushrealty.local).

* Logical Organization: Built a scalable Organizational Unit (OU) hierarchy to separate corporate headquarters (PRG-HQ), regional branches (PRG-Branches), and external contractors (PRG-External) (See Figure 2.1).

* CLI Account Automation: Engineered and executed command-line scripts to rapidly provision 7 distinct employee user profiles into the directory database, standardizing logon naming conventions and initial credential baselines (See Figure 2.2).

## 🛡️ Phase 3: Advanced Group Policy Hardening (GPOs)
Custom Security Object Baseline: Isolated custom domain rules from default system templates by engineering a dedicated Group Policy Object (PRG-Security-Policy) linked directly to the root domain.

* Granular Password Lifecycle Control: Enforced strict corporate credential safety windows by establishing a 90-day maximum password age (forcing rotation) and a 30-day minimum password age (preventing rapid reuse back-to-back), paired with a 12-character minimum length and complexity mandate (See Figure 3.2).

* Brute-Force Lockout Defense: Mitigated credential-stuffing and brute-force risks by configuring an Account Lockout Threshold of 5 invalid logon attempts, successfully forcing updates live via command-line updates (gpupdate /force) (See Figure 3.1).

* Desktop & Control Panel Lockdown: Hardened user desktop environments across the enterprise by pushing domain-wide restrictions that blocked access to the Windows Control Panel/Settings app and enforced a standardized corporate desktop wallpaper.

## 📁 Phase 4: Enterprise File Services & NTFS Security
Shared Infrastructure: Built and provisioned a central network repository by creating a shared corporate directory (PRG folder).

* Role-Based Privilege Lockout: Configured explicit NTFS permissions and network share folder settings to host enterprise assets, securing an Employee_Handbook.txt file by explicitly locking it down as Read-Only for standard users to protect regulatory data from alteration (See Figure 4.1).

## 🖥️ Phase 5: Remote Access & Support Engineering
Enterprise Client Deployment: Deployed TeamViewer as a third-party remote management solution to simulate a modern, cloud-brokered help desk support model.

* Cross-Platform Engineering: Established a secure remote pipeline bridging the physical macOS architecture (Client) to the virtualized Windows Server environment (Host) (See Figure 5.1).

* Unattended Access Validation: Configured automated startup services and permanent host credentials to support administrative maintenance without manual console intervention.

* System Architecture Documentation: Drafted and verified accurate technical documentation directly inside the remote host session to correctly define client-host relationships according to industry standards.


---
## 📸 Lab Deployment & Validation Gallery

This section compiles the technical documentation and visual validation of the Plush Realty Group enterprise lab environment.

### 💻 Infrastructure & Virtualization

#### Figure 1.1: Cloud Orchestration Environment
<p align="center">
  <img src="https://github.com/user-attachments/assets/2dc04a4b-98f7-40ed-a6de-d74f57765581" width="750" alt="GCP and VM Orchestration">
</p>
<p align="center"><i>Cross-platform orchestration—deploying and running Windows Server 2022 instances inside Google Cloud Platform (GCP) Compute Engine using a macOS host endpoint.</i></p>

---

### 🏛️ Directory Services & Automation

#### Figure 2.1: Active Directory OU Hierarchy
<p align="center">
  <img src="https://github.com/user-attachments/assets/5c940772-e23d-4804-8e63-3b4b5b05e4b8" width="750" alt="Active Directory OU Structure">
</p>
<p align="center"><i>Logical organization within Active Directory Users and Computers (ADUC), establishing structured OUs for Corporate Headquarters (PRG-HQ), Regional Branches (PRG-Branches), and External Contractors.</i></p>

---

#### Figure 2.2: Bulk User Provisioning via Command Line
<p align="center">
  <img src="https://github.com/user-attachments/assets/f5d46f5b-c2e3-4017-ade7-1d38f520b8da" alt="Bulk User Provisioning Script">
</p>
<p align="center"><i>Leveraging command-line automation for bulk object ingestion and standardized identity provisioning across target organizational groups.</i></p>

---

### 🔐 Group Policy Objects & Security Hardening

#### Figure 3.1: Account Lockout Policy Enforcement
<p align="center">
  <img src="https://github.com/user-attachments/assets/7d426de2-a735-4a1d-b85b-2636a66ba15d" width="750" alt="Account Lockout Policy">
</p>
<p align="center"><i>Hardening identity infrastructure by implementing an Account Lockout Policy under the custom PRG-Security-Policy GPO to mitigate brute-force and credential-stuffing attacks.</i></p>

---

#### Figure 3.2: Password Complexity & Lifecycle Controls
<p align="center">
  <img src="https://github.com/user-attachments/assets/6bb49d6a-1bce-4d83-b309-fe6968c26866" width="750" alt="Password Password Complexity Policy">
</p>
<p align="center"><i>Configuring robust password enforcement rules, establishing a 12-character minimum length restriction, and mandating strict complexity validation for domain identities.</i></p>

---

### 📂 File Services & Access Auditing

#### Figure 4.1: Effective Access Security Verification
<p align="center">
  <img src="https://github.com/user-attachments/assets/1e3c3fbc-a2b5-44e0-b094-c740abe67f5e" width="750" alt="Effective Access Share Auditing">
</p>
<p align="center"><i>Auditing shared file structures using Effective Access verification to validate strict NTFS security isolation and prevent unauthorized data privilege leakage.</i></p>

---

### 🌐 Technical Support & Remote Operations

#### Figure 5.1: Cross-Platform Remote Support Session
<p align="center">
  <img src="https://github.com/user-attachments/assets/f8630ab5-6824-4e99-8232-bbf90b522ff1" alt="TeamViewer Remote Desktop Verification">
</p>
<p align="center"><i>Simulating an enterprise support desk scenario—utilizing a secure, brokered TeamViewer tunnel to establish remote host control from a macOS technician endpoint to the target cloud VM node.</i></p>

---

### 🛠️ Key Skills Demonstrated

* **Systems Administration & Virtualization:** Windows Server 2022 Deployment | macOS Management Endpoint Operations | GCP Compute Engine Orchestration
* **Identity & Access Management (IAM):** Active Directory Domain Services (AD DS) | Organizational Unit (OU) Architecture | Bulk User Ingestion & Provisioning Automation
* **Group Policy Management (GPOs):** Custom Security Object Baselines | Password Complexity Enforcement | Account Lockout Defense & Cybersecurity Hardening
* **Network & Support Engineering:** Cross-Platform Remote Support (TeamViewer) | Secure Remote Pipeline Architecture | NTFS File Permissions & Share Access Auditing
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
