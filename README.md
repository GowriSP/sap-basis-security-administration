## SAP BASIS Security Administration

## Overview

This repository provides a practical guide to SAP BASIS Security Administration activities. It covers user management, role administration, authorization troubleshooting, password policies, audit logging, and SAP security best practices used in real-time SAP landscapes.

## Topics Covered

- User Administration (SU01)
- Mass User Maintenance (SU10)
- Role Administration (PFCG)
- Profile Management
- Password Policy Configuration
- User Lock and Unlock Procedures
- Authorization Troubleshooting (SU53, ST01)
- Security Audit Log Monitoring (SM19, SM20)
- Security Best Practices

## Key SAP Transactions

| T-Code | Purpose |
|---------|---------|
| SU01 | User Administration |
| SU10 | Mass User Maintenance |
| PFCG | Role Maintenance |
| SU53 | Authorization Analysis |
| ST01 | Authorization Trace |
| SM19 | Security Audit Setup |
| SM20 | Security Audit Analysis |
| SCC4 | Client Administration |

## User Administration

### User Types

- Dialog User
- System User
- Communication User
- Service User
- Reference User

### Common Activities

- User Creation
- User Modification
- Password Reset
- User Lock/Unlock
- Role Assignment

## Role Administration

### Role Types

- Single Role
- Composite Role
- Derived Role

### Responsibilities

- Create Roles
- Maintain Authorization Objects
- Generate Profiles
- Assign Roles to Users
- Transport Roles Across Systems

## Authorization Troubleshooting

### SU53 Analysis

1. Execute transaction SU53 immediately after authorization error.
2. Identify missing authorization object.
3. Update role in PFCG.
4. Generate authorization profile.
5. Reassign role and validate access.

### ST01 Trace

- Activate Authorization Trace.
- Reproduce the issue.
- Analyze failed authorization checks.
- Update required authorizations.

## Security Audit

### Security Audit Log

#### Configuration
- SM19

#### Analysis
- SM20

### Audit Activities

- Monitor User Logins
- Track Critical Transactions
- Review Failed Logon Attempts
- Audit Security Events

## Password Policy

### Recommended Practices

- Enforce Password Complexity
- Configure Password Expiry
- Prevent Password Reuse
- Lock Users After Failed Attempts

## Security Best Practices

- Apply Least Privilege Principle
- Remove Inactive Users
- Review Critical Authorizations Periodically
- Enable Security Audit Logs
- Monitor Emergency Users
- Perform Regular Access Reviews

## Author

**Gowri S**  
SAP BASIS Consultant
