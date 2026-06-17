# User Administration in SAP

## Overview

User Administration is a core SAP BASIS security activity responsible for managing user accounts, authorizations, passwords, and access controls within the SAP landscape.

## Transaction Code

| T-Code | Description |
|---------|------------|
| SU01 | User Maintenance |
| SU10 | Mass User Maintenance |
| SUIM | User Information System |
| SLICENSE | License Administration |

---

## User Types in SAP

### Dialog User
- Interactive system access
- Used by end users
- Password expiration applicable

### System User
- Background processing
- RFC communications
- No interactive logon

### Communication User
- External system integration
- RFC connections
- Password managed manually

### Service User
- Shared access users
- Anonymous logon possible
- No individual assignment

### Reference User
- Authorization assignment only
- Cannot log on directly

---

## User Creation Process

### Step 1
Execute Transaction:

```text id="c7r8s9"
SU01
```

### Step 2

Enter User ID and click Create.

### Step 3

Maintain:

- First Name
- Last Name
- Email Address
- User Group
- Department

### Step 4

Assign Required Roles.

### Step 5

Generate Password and Save User.

---

## Password Reset Process

### Steps

1. Open SU01
2. Enter User ID
3. Click Change Password
4. Set Temporary Password
5. Save Changes

---

## User Lock and Unlock

### Manual Lock

```text id="a1b2c3"
SU01 → Logon Data → Lock User
```

### Manual Unlock

```text id="d4e5f6"
SU01 → Logon Data → Unlock User
```

### Common Reasons

- Multiple Failed Logins
- Security Policy Violation
- User Request
- Audit Requirement

---

## Mass User Maintenance

### Transaction

```text id="g7h8i9"
SU10
```

### Activities

- Mass Role Assignment
- Mass User Lock
- Mass User Unlock
- Password Reset
- User Data Update

---

## User Information System

### Transaction

```text id="j1k2l3"
SUIM
```

### Reports

- Users by Role
- Users by Profile
- Locked Users
- Expired Users
- Critical Authorization Reports

---

## Common Administration Tasks

### Daily Activities

- Create New Users
- Modify Existing Users
- Reset Passwords
- Unlock Users
- Role Assignment Validation

### Weekly Activities

- Review Locked Users
- Review Inactive Users
- Authorization Verification
- User Access Validation

---

## Common Interview Questions

### What is SU01?

SU01 is used for SAP User Administration activities such as user creation, modification, password reset, role assignment, and user locking/unlocking.

### Difference Between Dialog and System User?

| Dialog User | System User |
|------------|------------|
| Interactive Login | No Interactive Login |
| Used by End Users | Used for Background Processing |
| Password Expiry Enabled | Password Expiry Not Applicable |

### What is SU10?

SU10 is used for mass maintenance of SAP users.

### What is SUIM?

SUIM provides user-related reports and authorization analysis.

---

## Best Practices

- Follow Least Privilege Principle
- Remove Inactive Users Regularly
- Monitor Failed Logon Attempts
- Enforce Strong Password Policies
- Review Critical Users Periodically
- Maintain Proper Role Assignments

---

## Author

**Gowri S**  
SAP BASIS Consultant
