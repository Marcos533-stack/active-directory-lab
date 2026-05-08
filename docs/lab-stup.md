# Active Directory Lab Setup

## Lab Overview

This lab simulates a basic corporate Active Directory environment using VirtualBox and Windows Server.

The objective of the project is to practice:

- Active Directory Domain Services (AD DS)
- DNS configuration
- User and group management
- Organizational Units (OU)
- Group Policy Objects (GPO)
- Domain-joined client administration

---

# Environment

## Virtualization Platform

- VirtualBox

## Virtual Machines

| Machine | Role | Operating System |
|---|---|---|
| DC01 | Domain Controller | Windows Server 2022 |
| CLIENT01 | Domain Client | Windows 10 |

---

# Network Configuration

| Machine | IP Address | Role |
|---|---|---|
| DC01 | 192.168.1.10 | DNS / Domain Controller |
| CLIENT01 | DHCP / Static | Domain Client |

Domain Name:

```text
corp.local
```

---

# Domain Controller Configuration

The following roles and services were installed on DC01:

- Active Directory Domain Services (AD DS)
- DNS Server

The server was promoted to a domain controller for the domain:

```text
corp.local
```

---

# Organizational Units (OU)

The following Organizational Units were created:

- IT
- HR

These OUs were used to organize users and apply department-specific GPOs.

---

# Users and Groups

## Users

| Username | Department |
|---|---|
| mruiz | Administration |
| it.support | IT |
| hr.user | HR |

## Security Groups

| Group Name | Scope | Type |
|---|---|---|
| IT | Global | Security |
| HR | Global | Security |

---

# Group Policy Objects (GPO)

## HR Policy

Applied restrictions:
- Control Panel access disabled

## IT Policy

Applied configurations:
- Administrative access policies enabled

---

# Domain Join

The Windows 10 client machine was successfully joined to the domain:

```text
corp.local
```

Users were able to authenticate using domain credentials.

Example:

```text
CORP\it.support
```

---

# Screenshots

Project screenshots are available in the `/screenshots` directory.

Included screenshots:
- Domain Controller configuration
- Active Directory Users and Computers
- GPO configuration
- Domain-joined client
- Domain user login

---

# Lessons Learned

This lab helped reinforce practical knowledge in:

- Active Directory administration
- Windows Server management
- Group Policy deployment
- Domain infrastructure basics
- User and permission management
- Virtualized enterprise environments