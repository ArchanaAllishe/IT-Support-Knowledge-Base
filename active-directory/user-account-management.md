# Active Directory User Account Management

## Purpose

This document outlines common user account administration tasks performed in Active Directory. It serves as a reference for managing user accounts, access permissions, and account lifecycle activities in a Windows domain environment.

---

## Scope

This guide applies to common Active Directory user administration tasks, including:

* User account updates
* Password resets
* Account lockout resolution
* Account enable/disable
* Security group management
* Organizational Unit (OU) management
* Employee onboarding
* Employee offboarding

---

# Common User Administration Tasks

| Task                    | Description                                                               |
| ----------------------- | ------------------------------------------------------------------------- |
| Create User Account     | Create a new user account following organizational naming standards.      |
| Reset Password          | Reset a user's password after verifying identity.                         |
| Unlock Account          | Unlock an account locked due to failed sign-in attempts.                  |
| Enable Account          | Re-enable a disabled user account.                                        |
| Disable Account         | Disable accounts for terminated employees or extended leave.              |
| Update User Information | Modify job title, department, manager, office location, or phone number.  |
| Manage Group Membership | Add or remove users from security or distribution groups.                 |
| Move User to an OU      | Place users in the appropriate Organizational Unit for policy management. |

---

# Password Reset Procedure

## When to Use

* User forgot password
* Password expired
* Temporary password required
* Password compromised

## Procedure

1. Verify the user's identity according to company policy.
2. Open **Active Directory Users and Computers (ADUC)**.
3. Locate the user account.
4. Right-click the account and select **Reset Password**.
5. Enter a temporary password.
6. Select **User must change password at next logon**.
7. Provide the temporary password securely to the user.

## Verification

Confirm that:

* The user can sign in successfully.
* The password is changed.
* The account is no longer locked.

---

# Account Lockout Resolution

## Common Causes

* Incorrect password entered multiple times
* Cached credentials
* Mobile device using an old password
* Outlook repeatedly attempting authentication
* Mapped network drives using outdated credentials

## Resolution

1. Verify the user's identity.
2. Open the user account in ADUC.
3. Unlock the account.
4. Confirm the user can sign in.
5. Investigate the root cause to prevent repeated lockouts.

---

# Updating User Information

Common updates include:

* Display name
* Department
* Job title
* Manager
* Office location
* Telephone number
* Email aliases (where applicable)

Always verify the requested changes before making updates.

---

# Security Group Management

Security groups are commonly used to provide access to:

* Shared folders
* Network printers
* Business applications
* Departmental resources

## Procedure

1. Verify the access request has been approved.
2. Locate the user account.
3. Open **Properties**.
4. Select the **Member Of** tab.
5. Add or remove the appropriate group.
6. Save the changes.
7. Ask the user to sign out and sign back in if necessary.

---

# Employee Onboarding

Typical onboarding tasks include:

* Create user account
* Assign username
* Set temporary password
* Add required security groups
* Configure email account
* Assign Microsoft 365 license (if applicable)
* Verify initial sign-in

---

# Employee Offboarding

Typical offboarding tasks include:

* Disable the user account
* Remove unnecessary group memberships
* Reset the password if required by policy
* Document account status
* Archive data according to organizational procedures

---

# Best Practices

* Verify user identity before making account changes.
* Follow the principle of least privilege.
* Document significant account modifications.
* Avoid sharing passwords through unsecured communication methods.
* Confirm changes with the user whenever possible.

---

# User Communication

### Password Reset

> Your password has been reset. Please sign in using the temporary password provided and create a new password when prompted.

### Group Membership Update

> Your account permissions have been updated. Please sign out and sign back in for the changes to take effect.

### Account Unlock

> Your account has been unlocked. Please try signing in again. If the issue continues, contact IT Support for additional assistance.

---

# Related Articles

* Windows User Profile Troubleshooting
* Microsoft Office Installation
* Microsoft Outlook Configuration
* Password Reset and Account Lockout
* User Onboarding Checklist
