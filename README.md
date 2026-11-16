# 🧪 Active Directory Home Lab – Beginner Edition

Spin up your own mini enterprise IT environment — all from a single machine.

This beginner-friendly lab walks you through installing and configuring Active Directory, DNS, DHCP, Group Policy, and more using VMware Workstation Pro. No prior Virtual Machine or Active Directory experience needed.


## Setup using Silicon M1-M4 MacOS processers

Hypervisors that can be used doesn't matter (some have different caveats and features)
 - VirtualBox or VMWare Fusion, you can use either one
 - VMWare Fusion offers weirdly easier way to get a Windows 11 pro or enterprise ISO file that works for MacOS.

Anyone using MacOS computers after Apple transitioned from Intel-based processors to Silicon ARM M1-M4 will face troubles running the Windows Server 19 Evaluation ISO file
 - Users have requested for an ARM-compatible iso file but isn't available in Windows Evaluation Center or Insider Program. 

Workarounds for Windows Server ARM64 compatiblity: 

- workaround 1: using UTM to emulate Windows Server 2019 so it can interact with your virtualized Windows pro 10 or 11 client. Window 11 is used for this example. 

- workaround 2:
  - using UUP Dump to get an ARM64 iso (alot of technical steps involved that may be overwhelming and confusing)
    - involves installation of multi-protocol & multi-source command-line download utility [aria2](https://aria2.github.io/)
    - There are builds of 2025 Windows Server with ARM64 which can also be looked into
      - This forum post goesinto more details https://forums.macrumors.com/threads/windows-server-2025-arm-on-mac.2423766/ 
   


Resources for the workarounds:
- https://techcommunity.microsoft.com/discussions/windows11/is-uup-dump-a-legitimate-tool-for-windows-iso-download/4547467/replies/4547479
- https://4sysops.com/archives/download-the-windows-server-2025-iso-for-intel-x64-and-arm-arm64/


---

## 📌 What This Lab Includes

- 🖥️ Two virtual machines:
  - `DC01`: Windows Server 2019 domain controller
  - `CLIENT01`: Windows 10 or 11 workstation 
- 🌐 Networking using VMware NAT + Host-Only adapters
- 🧱 Domain setup with `corp.local`
- 🔐 Active Directory user and group management
- 🧠 Group Policy walkthroughs

---

## 🛠 Requirements

### 📅 Software Downloads
- 🔗 [VMware Workstation Pro](https://www.vmware.com/products/workstation-pro.html)
- 🔗 [UTM for MacOS Operating Systems](https://getutm.app/)
- 🔗 [Windows Server 2019 Evaluation ISO](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019)  
- 🔗 [Windows 10 Evaluation ISO](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-10-enterprise)  

### 💾 System Requirements
- Minimum: **4GB RAM** (8GB recommended)
- At least **100GB of free disk space**
- 🧠 Basic familiarity with Windows and networking settings

---

## 📘 Start Building Your Lab

This project is divided into two parts:

### 🔧 [Lab Setup Guide](./lab-setup-guide.md)
🚧 Set up your lab environment from scratch using VMware Workstation Pro.

### 🎯 [Active Directory Tasks Walkthrough](./ad-basic-tasks.md)
💡 Practice managing users, groups, OUs, and GPOs!

---

## 🚀 Why This Lab?

This lab is built for learners who:

- 👨‍💻 Want hands-on practice with a real Windows domain setup  
- 🙅‍♀️ Are tired of vague instructions and confusing jargon  
- 🎯 Are prepping for certs or interviews and need real-world context

---

## 📸 Screenshots

Included throughout both the [Lab Setup Guide](./lab-setup-guide.md) and the [Active Directory Tasks Walkthrough](./ad-basic-tasks.md) — no guesswork required.

---

## ☕ Support & Subscribe

If this project helps you out:

- ⭐ Star this repo
- 🔧 Suggest improvements or ask questions via [issues](https://github.com/learnbuilddeploylabs/active-directory-home-lab/issues)
- ☕ [Buy me a coffee](https://buymeacoffee.com/learnbuilddeploy)
- 📺 [Subscribe on YouTube](https://youtube.com/@learnbuilddeploy)

---

## 📬 Contact

Got a question or hit a snag?

- 💬 [Open an issue](https://github.com/learnbuilddeploylabs/active-directory-home-lab/issues)
- 📧 Email: learnbuilddeploylabs@gmail.com

---

## 🙋‍♂️ About the Author

This project was created by **Rob Merrill**, an aspiring cybersecurity professional documenting hands-on labs to help others learn by doing.

- 🎓 Career-changer with a passion for IT and cybersecurity
- 📺 Creator of [Learn. Build. Deploy.](https://youtube.com/@learnbuilddeploy)
- 🧰 Always building — always sharing

---

**Cheers, and happy labbing!** 🥃

