# 🧩 Nagios-Compatible Plugins

A public collection of **custom Nagios-compatible plugins** crafted to monitor diverse systems, applications, and services.  
Each plugin is designed for **reliability, portability**, and **easy integration** with Nagios Core and compatible systems like **Icinga**, **Naemon**, opsview, zabbix or any other nagios plugins compatible monitoring tool.

---

## 📋 Overview

This repository contains plugins I’ve developed over time for various use cases, including:

- System health checks (CPU, memory, disk, processes)
- Network and service availability
- Application-specific monitoring
- API and endpoint checks
- Security and compliance status
- Custom business logic monitoring

Each plugin follows the Nagios plugin development guidelines and returns standard exit codes:
- `0` → OK  
- `1` → WARNING  
- `2` → CRITICAL  
- `3` → UNKNOWN

---

## ⚙️ Usage

Each plugin can be executed directly from the command line or called by the monitoring tool.

Example:
```bash
/usr/lib/nagios/plugins/check_custom_service.sh -H example.com -w 80 -c 90
/opt/opsview/monitoringscripts/plugins/check_custom_service.sh -H example.com -w 80 -c 90

