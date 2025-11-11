# Intelligent Linux Maintenance Utility (C++ Project)

### Automated System Hygiene & Backup Manager for Linux

---

##  Overview
This project is a modern C++20 based command line tool that automates daily Linux maintenance operations such as backup creation, junk cleanup, system information display and disk usage monitoring.  
This tool reduces repeated manual administration work and keeps the system clean and organized.


---

##  Features
- Shows CPU info, RAM usage and System uptime
- Creates timestamp based backup folders
- Cleans temporary user junk from `/tmp`
- Displays disk usage summary
- Auto deletes logs + backups older than 7 days
- Fully menu driven CLI program

---

##  Tech Stack

| Area | Technology Used |
|------|-----------------|
| Language | C++20 |
| Compiler | g++ |
| Operating System | Linux |
| Libraries | `<filesystem>`, `<chrono>`, Standard Library |

---

##  System Flow
1. Program launches with menu interface  
2. User selects required option  
3. Selected module executes logic  
4. Logs / backup / cleanup tasks executed  
5. Auto clean periodically removes stale data

---

##  Installation & Run ## Folder Structure

```bash
git clone <your_repository_link>
cd <project_folder_name>
g++ -std=c++20 main.cpp -o maintainer
./maintainer


---
project_folder_name/
│
├── src/              # Source code files (if modularized)
├── backups/          # Auto-generated backups stored here
├── logs/             # Log files and system cleanup records
├── main.cpp          # Main source file
└── README.md         # Documentation file

