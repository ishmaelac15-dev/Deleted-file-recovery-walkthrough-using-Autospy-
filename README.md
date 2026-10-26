# Deleted-file-recovery-walkthrough-using-Autospy

## Objective
- Build a controlled test environment and create known evidence
- Acquire a forensic image and preserve its integrity with hashing
- Locate deleted files using Autopsy file system
- Recover files and verify them against the original SHA-256 hashes
-Document findings
## Lab Environment
| Component | Details |
|-----------|---------|
| Hypervisor | Oracle VirtualBox (version: _TBD_) |
| Evidence machine | Windows 10 VM with a 2 GB secondary NTFS virtual disk |
| Analysis machine | Debian (version: _TBD_) VM |
| Forensic software | Autopsy (version: _TBD_) with The Sleuth Kit |
| Imaging | FTK Imager or `VBoxManage clonemedium` (raw/dd) |
| Hashing | PowerShell `Get-FileHash` / Linux `sha256sum` |
## Test Data
No real or personal data is used. 
| File | Type | Original SHA-256 | Deletion method | Recovered? | Hash match? |
|------|------|------------------|-----------------|------------|-------------|
| `Dog.jpg` | Image | _TBD_ | Recycle Bin, then emptied | _TBD_ | _TBD_ |
| `Cat.jpg` | Image| _TBD_| Recycle Bin, then emptied| _TBD_| _TBD|
| `Journal.txt` | Text | _TBD_ | Delete, then overwritten | _TBD_ | _TBD_ |
| `In-n-Out.pdf` | PDF | _TBD_ | Shift+Delete | _TBD_ | _TBD_ |
## Repository Structure
```
autopsy-deleted-file-recovery/
├── README.md
├── walkthrough.md
├── screenshots/        # Numbered to match walkthrough steps
├── evidence-notes/     # Hash logs, file listings, timeline notes
└── LICENSE
```
## Disclaimer
This project was performed in an isolated lab for educational purposes using only data I created.
