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

##  Installation & Run

```bash
git clone <your_repository_link>
cd <project_folder_name>
g++ -std=c++20 main.cpp -o maintainer
./maintainer
```bash

## Folder Structure
|
|-- src/
|-- backups/
|-- logs/
|-- main.cpp
|-- README.md

---


## Usage Guide

| Operation        | Action                                                    |
| ---------------- | --------------------------------------------------------- |
| System Info      | Choose System Info option                                 |
| Backup           | Choose Backup option to auto create timestamp folder      |
| Clean Temp Files | Select Clean Temp option                                  |
| Disk Usage       | Select Disk Usage option                                  |
| Auto Cleaner     | Automatically deletes old files (no user action required) |


---

Future Improvements
Add monitoring TUI dashboard
Add cloud sync option for secure backup
Provide GUI front-end version

---

Contribution
Contributions & PRs are welcome.

