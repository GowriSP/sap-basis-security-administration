# Audit and Security Checks in SAP

## Overview

SAP Security Auditing helps organizations monitor user activities, identify security risks, ensure compliance, and detect unauthorized system access.

Regular security checks are essential for maintaining a secure SAP landscape.

## Important Transactions

| T-Code | Description |
|---------|------------|
| SM19 | Security Audit Log Configuration |
| SM20 | Security Audit Log Analysis |
| SUIM | User Information System |
| SU01 | User Administration |
| ST01 | System Trace |
| SM21 | System Log |
| RZ10 | Profile Maintenance |
| RZ11 | Profile Parameter Display |

---

## Security Audit Log

### Configuration

Transaction:

```text
SM19
```

Purpose:

- Enable Security Audit Logging
- Configure Audit Events
- Monitor Critical Activities

Events Monitored:

- User Logon
- User Logoff
- Failed Logon Attempts
- Transaction Execution
- User Lock/Unlock Activities
- RFC Logins

---

## Security Audit Analysis

Transaction:

```text
SM20
```

Purpose:

- Review Security Events
- Investigate Suspicious Activities
- Generate Audit Reports

Common Checks:

- Failed Login Attempts
- Unauthorized Access Attempts
- Critical Transaction Usage
- User Activity Monitoring

---

## User Security Review

Transaction:

```text
SUIM
```

Checks:

### Locked Users

```text
SUIM
↓
Users
↓
By Logon Data
```

### Users Without Roles

```text
SUIM
↓
Users
↓
Users By Complex Selection Criteria
```

### Critical Users

Review:

- SAP*
- DDIC
- Emergency Users
- Firefighter IDs

---

## Failed Login Monitoring

Transactions:

```text
SM20
SM21
```

Review:

- Repeated Failed Logins
- Unauthorized Login Attempts
- User Lock Events

Purpose:

- Detect Brute Force Attacks
- Identify Security Risks

---

## Role and Authorization Review

Transactions:

```text
PFCG
SUIM
```

Checks:

- Critical Authorizations
- Unused Roles
- Excessive Privileges
- Segregation of Duties Issues

---

## System Log Monitoring

Transaction:

```text
SM21
```

Review:

- Security Errors
- User Lock Events
- System Warnings
- Authorization Failures

Benefits:

- Early Issue Detection
- Security Monitoring
- Compliance Support

---

## Authorization Audit

Transactions:

```text
SU53
ST01
SU56
```

Purpose:

- Identify Missing Authorizations
- Analyze Access Issues
- Verify User Permissions

---

## Daily Security Checklist

### User Administration

- Review Locked Users
- Review Failed Login Attempts
- Verify Critical User Activity

### System Monitoring

- Check SM21 Logs
- Check Security Audit Logs
- Verify Background Jobs

### Authorization Monitoring

- Analyze SU53 Issues
- Review Critical Roles
- Validate User Access

---

## Weekly Security Checklist

- Review Inactive Users
- Remove Unused Roles
- Review Critical Authorizations
- Analyze Audit Logs
- Validate Emergency Access Users
- Check Password Compliance

---

## Monthly Security Checklist

- User Access Review
- Role Review
- Compliance Validation
- Security Audit Report Generation
- Segregation of Duties Analysis

---

## Common Interview Questions

### What is SM19?

SM19 is used to configure the SAP Security Audit Log.

### What is SM20?

SM20 is used to analyze Security Audit Log entries.

### Why Perform Security Audits?

Security audits help detect unauthorized access, monitor user activities, and ensure compliance.

### Which Transaction Is Used To Review Users?

```text
SUIM
```

### Which Transaction Is Used To Monitor Security Events?

```text
SM20
```

---

## SAP Security Best Practices

- Enable Security Audit Logging
- Review Critical Users Regularly
- Remove Inactive Users
- Monitor Failed Login Attempts
- Follow Least Privilege Principle
- Review Authorizations Periodically
- Perform Regular Compliance Checks
- Secure Emergency User Access

---

## Security Audit Flow

```text
User Activity
      ↓
Security Audit Log (SM19)
      ↓
Audit Analysis (SM20)
      ↓
Security Review
      ↓
Corrective Action
      ↓
Compliance Reporting
```

---

## Author

**Gowri S**  
SAP BASIS Consultant
