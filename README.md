# Active Directory Lab

![Windows Server](https://img.shields.io/badge/Windows%20Server-2022-blue)
![Active Directory](https://img.shields.io/badge/Active%20Directory-Lab-success)
![Platform](https://img.shields.io/badge/Platform-VirtualBox-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

A virtualized Active Directory lab environment built with Windows Server and VirtualBox.

This project simulates a basic corporate infrastructure focused on:

- Active Directory Domain Services (AD DS)
- DNS configuration
- User and group administration
- Organizational Units (OU)
- Group Policy Objects (GPO)
- Domain-joined Windows clients

---

# Lab Architecture

```text
[ CLIENT01 ]
Windows 10 Client
        |
        |
[ DC01 ]
Windows Server 2022
AD DS | DNS | GPO
```

---

# Technologies Used

- Windows Server 2022
- Windows 10
- VirtualBox
- Active Directory Domain Services (AD DS)
- DNS
- Group Policy Management

---

# Features Implemented

- Domain Controller deployment
- Domain creation (`corp.local`)
- DNS configuration
- User and security group management
- Organizational Units (OU)
- Group Policy Objects (GPO)
- Domain client integration
- Domain authentication testing

---

# Security Groups

| Group | Scope | Type |
|---|---|---|
| IT | Global | Security |
| HR | Global | Security |

---

# Group Policies

## HR
- Control Panel access disabled

## IT
- Administrative access policies enabled

---

# Screenshots

## Domain Controller

![Domain Controller](screenshots/domain-controller.png)

---

## Active Directory Users and Computers

![AD Users and Computers](screenshots/active-directory-users.png)

---

## Group Policy Configuration

![Group Policy](screenshots/group-policy.png)

---

## Domain-Joined Client

![Joined Client](screenshots/joined-client.png)

---

# Project Structure

```text
active-directory-lab/
│
├── README.md
├── docs/
│   └── lab-setup.md
│
└── screenshots/
    ├── domain-controller.png
    ├── active-directory-users.png
    ├── group-policy.png
    └── joined-client.png
```

---

# Documentation

Detailed lab configuration documentation is available here:

```text
docs/lab-setup.md
```

---

# Skills Practiced

- Windows Server administration
- Active Directory management
- GPO deployment
- DNS configuration
- Domain administration
- Virtualized infrastructure management

---

# Purpose of the Project

This lab was created to strengthen practical skills related to enterprise Windows environments and system administration workflows commonly found in corporate IT infrastructures.
