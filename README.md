# mysql-it-support-db
Production-ready MySQL database setup, table schema, and automated bash backup workflow for IT support tracking on Ubuntu Linux.

# MySQL IT Support Database

A practical MySQL database administration project running on Ubuntu Linux.
This project demonstrates MySQL installation, service management, database and table creation, basic SQL operations, security configuration, database backup using `mysqldump`, and Bash scripting.

## Project Objectives

The main objectives of this project are:

- Install and configure MySQL Server on Ubuntu
- Manage MySQL using systemd
- Create and manage databases
- Create tables and insert data
- Perform basic SQL operations
- Secure the MySQL installation
- Take database backups using `mysqldump`
- Automate database backup using Bash
- Schedule backups using cron
- Document the complete process

## Technologies Used

- Ubuntu Linux
- MySQL Server
- SQL
- Bash Shell
- systemd
- mysqldump
- cron
- Git & GitHub

## Repository Structure

```text
mysql-it-support-db/
│
├── README.md
│
├── scripts/
│   ├── setup_db.sql
│   └── backup_db.sh
│
├── docs/
│   └── screenshots/
│
└── backups/
    └── .gitkeep
