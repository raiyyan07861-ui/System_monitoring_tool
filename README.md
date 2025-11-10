Intelligent Linux Maintenance Utility (C++ Project)
Automated System Hygiene & Backup Manager for Linux
Table of Contents

Overview

Features

Tech Stack

System Flow Summary

Setup & Installation

Usage Instructions

Directory Structure

Future Enhancements

Contribution

License

Overview

This project is a C++20 based terminal application that simplifies routine Linux administration and housekeeping tasks.
It helps users quickly view system insights, remove unnecessary temporary files, manage disk usage, maintain logs, and perform timestamp-based backups — all from a single unified menu driven program.

This tool was initially prototyped using a Bash shell-script implementation and later refactored to modern C++ using <filesystem> for improved reliability, portability and performance.

Features

Display live system details (CPU info, RAM usage, Uptime)

Generate secure automatic file backups with timestamp folder creation

Clean temporary junk files from /tmp

Show disk usage summary for quick decision making

Auto delete outdated backups & logs older than 7 days

Lightweight CLI + low resource consumption suitable for everyday use

Tech Stack
Area	Technology Used
Language	C++20
Libraries	filesystem, chrono, STL
OS Environment	Linux distributions (tested on Ubuntu based variants)
Compiler	g++
System Flow Summary

Start program → menu screen displayed

User selects the action they want to perform

Corresponding module executes (backup/info/cleanup/storage-report)

Program maintains logs for transparency

Old stale data is auto removed periodically

Setup & Installation
git clone <your >
cd <project>

g++ -std=c++20 main.cpp -o maintainer
./maintainer

Usage Instructions
Task	How to Perform
Check system info	Run tool → choose option for System Stats
Create backup	Select Backup option → files get copied with timestamp
Clean temp space	Select Clean option to remove user temporary files
View disk usage	Select Disk Usage option
Auto cleanup	Automatically handled inside code (7 days)
Directory Structure
|
|-- src/            # source files if separated
|-- backups/        # auto created folders for backups
|-- logs/           # logging of operations performed
|-- main.cpp
|-- README.md

Future Enhancements

Add live usage monitoring graphs (ncurses / tui based)

Add user level backup include/exclude filters

Optional cloud backup sync (Drive/S3)

Web dashboard front-end in future version

Contribution

Pull Requests / Issue reporting is appreciated.
Follow standard formatting (clang-format preferred).

License

MIT License.
