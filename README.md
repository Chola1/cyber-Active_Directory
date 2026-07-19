# cyber-Active_Directory

# Active Directory Administration & Group Policy

This section documents hands-on configuration of **Active Directory Domain Services (AD DS)** and **Group Policy Objects (GPOs)** in a Windows Server home lab. The objective was to understand how organizations manage users, enforce security policies, and control access to enterprise resources through centralized administration.

This Active Directory lab serves as the foundation for Windows Security Event Log collection and authentication monitoring in my Splunk SOC lab.
---

## #1 Controlling User Logon Hours

### Objective
Restrict user authentication to approved business hours.

### Configuration

Configured **Logon Hours** for a domain user to allow authentication only during predefined time periods.

### What it does

This configuration prevents users from logging on outside approved working hours, reducing the risk of unauthorized access and strengthening access control. Logon restrictions are commonly used in enterprise environments for privileged or shift-based accounts.

---

## #2 Creating Organizational Units, Security Groups, and Users

### Objective
Organize users and resources using Active Directory.

### Configuration

Created Organizational Units (OUs), user accounts, computer containers, and security groups to simulate a structured enterprise Active Directory environment.

### What it does

Organizing resources into OUs allows administrators to delegate administration, simplify management, and apply Group Policies to specific users or computers. Security groups provide centralized permission management for shared resources.

---

## #3 Restricting Printer Installation Using Group Policy

### Objective
Prevent users from adding unauthorized printers.

### Configuration

Configured a Group Policy Object (GPO) to disable printer installation for users.

### What it does

Restricting printer installation helps reduce unauthorized device usage and enforces endpoint security policies. Group Policy enables administrators to centrally apply these restrictions across multiple domain-joined systems.

---

## #4 Controlling Approved USB Printer Devices

### Objective
Allow only approved USB printers within the domain.

### Configuration

Configured the **Device Control Printing Restrictions** policy to specify approved USB printer devices.

### What it does

This policy restricts printing to authorized USB printers by allowing only approved device IDs. It helps organizations control peripheral usage, reduce unauthorized device connections, and improve endpoint security.

---

## Skills Demonstrated

- Active Directory Domain Services (AD DS)
- Organizational Unit (OU) Administration
- User & Group Management
- Security Group Administration
- Group Policy Management (GPO)
- Identity & Access Management (IAM)
- Windows Server Administration
- Access Control
- Endpoint Security
- Enterprise Policy Enforcement
