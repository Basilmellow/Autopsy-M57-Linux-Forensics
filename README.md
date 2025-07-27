# 🕵️‍♂️ Linux Digital Forensics with Autopsy – M57 Jean Case

**By Mohamed Basil (MindSec)**  


## 📁 Project Summary

This repository demonstrates a complete digital forensics investigation using **Autopsy (Linux version)** on the **M57 Jean case** from Digital Corpora. The goal was to uncover insider threat behavior using real forensic workflows, evidence analysis, and timeline reconstruction.

✅ Investigated on **Linux OS**  
✅ Real-world forensic disk image (public)  
✅ Screenshots, artifacts, reports included


## 📦 Case Details

**Scenario:**  
An employee of a fictional company, M57 Patents, is suspected of leaking sensitive documents via unauthorized USB activity. A disk image of their system was captured and assigned for forensic analysis.

**Source:**  
🔗 https://digitalcorpora.org/corpora/scenarios/m57-jean  


## 🛠️ Tools Used

- [Autopsy for Linux](https://sleuthkit.org/autopsy/)
- Sleuth Kit backend
- Linux OS (Kali)
- Screenshot tools (e.g., Flameshot)
- Custom Report Templates


## 🔍 Forensic Workflow

### ✅ 1. Case Setup  
- Created case in Autopsy Linux
- Imported `jean.E01` disk image
- Enabled modules: File Analysis, Recent Activity, Web Artifacts, Hashing, and Data Carving

### 🗂️ 2. File System Analysis  
- Identified deleted `.docx` and `.xls` files from `Documents`
- Found suspicious `.exe` in `/Users/Jean/Downloads`

### 🔌 3. USB Device History  
- Used Registry Viewer + Autopsy activity logs
- Confirmed SanDisk USB usage
- Correlated with file deletion events

### 🌐 4. Web Activity  
- Browsing history revealed use of file sharing platforms
- Keyword search: “delete evidence linux”, “cover tracks usb”

### 🕒 5. Timeline Reconstruction  
- Correlated timestamps: USB connection → file copy → deletion
- Used **Timeline View** to visualize events


## 📸 Evidence

Find screenshots in [`/Evidence_Screenshots`](./Evidence_Screenshots)

| Screenshot | Description |
|------------|-------------|
| `case-setup.png` | New Autopsy case created |
| `deleted-files.png` | Recovered deleted documents |
| `usb-history.png` | Registry and device logs |
| `timeline-view.png` | Full event correlation |


## 📑 Reports

Find all reports in [`/Reports`](./Reports):

- `M57_Executive_Report.pdf` – Non-technical summary with key findings
- `M57_Forensics_Technical_Report.pdf` – Detailed forensic analysis with hashes, timestamps, evidence


## 🧠 Lessons Learned

- Autopsy is powerful even on Linux systems
- Timeline correlation is key to establishing intent
- Registry + USB logs can confirm insider threat actions
- A well-documented case = proof of skill for recruiters


## 🔗 Connect

- 📄 Medium Blog Post: [Read on Medium]([https://medium.com/@yourusername/autopsy-m57-linux-forensics](https://medium.com/@Mindsec))
- 🔗 LinkedIn: [Connect with me](www.linkedin.com/in/mohamed-basil-966a8225a)


## 🙌 Final Note

This investigation project showcases real-world digital forensics capability using **only free tools on Linux**.  
If you're a recruiter, DFIR lead, or just learning, feel free to clone, fork, or reach out with questions.

**MindSec – Hacking the Future**

