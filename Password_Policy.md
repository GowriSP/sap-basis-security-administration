# Password Policy in SAP

## Overview

Password policies help secure SAP systems by enforcing strong authentication controls and reducing unauthorized access risks.

SAP provides profile parameters to manage password complexity, validity, lock periods, and login restrictions.

## Important Transactions

| T-Code | Description |
|---------|------------|
| RZ10 | Profile Maintenance |
| RZ11 | Display Profile Parameters |
| SU01 | User Administration |
| SU10 | Mass User Maintenance |

---

## Password Security Parameters

### Minimum Password Length

Parameter:

```text id="a1b2c3"
login/min_password_lng
```

Example:

```text id="d4e5f6"
8
```

Recommended:

```text id="g7h8i9"
8 - 12 Characters
```

---

### Password Expiration

Parameter:

```text id="j1k2l3"
login/password_expiration_time
```

Example:

```text id="m4n5o6"
90 Days
```

Purpose:

- Forces Regular Password Changes
- Improves Security Compliance

---

### Failed Login Attempts

Parameter:

```text id="p7q8r9"
login/fails_to_user_lock
```

Example:

```text id="s0t1u2"
5 Attempts
```

Purpose:

- Protects Against Brute Force Attacks
- Automatically Locks User

---

### Automatic Unlock Time

Parameter:

```text id="v3w4x5"
login/failed_user_auto_unlock
```

Purpose:

- Automatically Unlocks Users
- Reduces Administrative Effort

---

## Password Reset Process

Transaction:

```text id="y6z7a8"
SU01
```

Steps:

1. Open User
2. Select Logon Data
3. Enter Temporary Password
4. Save User
5. Inform User Securely

---

## User Lock and Unlock

### Lock User

```text id="b9c0d1"
SU01
↓
Logon Data
↓
Lock User
```

### Unlock User

```text id="e2f3g4"
SU01
↓
Logon Data
↓
Unlock User
```

---

## Password Best Practices

- Use Strong Passwords
- Enable Password Expiry
- Prevent Password Reuse
- Lock Users After Failed Attempts
- Avoid Shared Accounts
- Review Critical Users Regularly

---

## Common Interview Questions

### Which Parameter Controls Password Length?

```text id="h5i6j7"
login/min_password_lng
```

### Which Parameter Locks Users After Failed Attempts?

```text id="k8l9m0"
login/fails_to_user_lock
```

### Which Transaction Is Used for Password Reset?

```text id="n1o2p3"
SU01
```

### Why Are Password Policies Important?

Password policies protect SAP systems from unauthorized access and improve overall security compliance.

---

## Security Recommendations

- Minimum 8 Characters
- Regular Password Changes
- User Lock After Failed Attempts
- Monitor Critical Accounts
- Enforce Security Standards

---

## Author

**Gowri S**  
SAP BASIS Consultant
