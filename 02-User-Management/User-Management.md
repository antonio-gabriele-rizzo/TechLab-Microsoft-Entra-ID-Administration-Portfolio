# 02 - User Management

## Introduction

User management is one of the most common administrative responsibilities performed by IT Support Technicians, Service Desk Analysts, Junior Systems Administrators, and Microsoft 365 Administrators.

Microsoft Entra ID provides administrators with a central platform for managing user identities, account access, authentication settings, and user lifecycle operations.

This chapter demonstrates the complete lifecycle of a user account, including creation, modification, disabling, enabling, deletion, and restoration.

The purpose of this chapter is twofold:

1. Develop practical Microsoft Entra administration skills.
2. Create a reusable step-by-step reference guide for future use.

---

## Objectives

After completing this chapter, you should be able to:

- View existing users
- Create a new user account
- Configure user properties
- Disable a user account
- Re-enable a user account
- Delete a user account
- Restore a deleted user account
- Understand common user lifecycle administration tasks

---

## Prerequisites

Before starting this chapter, ensure you have:

- Access to Microsoft Entra Admin Center
- Administrative permissions
- An active Microsoft Entra tenant
- Existing user accounts within the tenant

---

# Understanding User Management

Users are the primary identity objects within Microsoft Entra ID.

Most day-to-day IT support activities involve user administration. Common examples include:

- Creating new employee accounts
- Updating user information
- Resetting passwords
- Disabling accounts
- Deleting accounts
- Restoring accidentally deleted accounts

Understanding these tasks is essential for entry-level IT support roles.

---

# Viewing Existing Users

## Navigation

Identity → Users → All Users

The All Users page displays all user accounts currently available within the tenant.

Information displayed includes:

- Display Name
- User Principal Name (UPN)
- User Type
- Domain
- Synchronisation Status

This page is commonly used by Service Desk Analysts when performing user administration tasks.

![Users Overview](screenshots/users-overview.png)

---

# Creating a New User

## Navigation

Identity → Users → New User

For this lab, a test account named **Helpdesk User** was created.

The following information was configured:

| Setting | Value |
|----------|----------|
| Display Name | Helpdesk User |
| Job Title | Helpdesk Technician |
| Department | IT Support |
| Office Location | London |

Before creating the account, review the configuration details.

![Create User Review](screenshots/create-user-review.png)

Select **Create** to create the account.

---

# Verifying User Creation

After the account has been created:

Identity → Users → All Users

Verify that Helpdesk User appears in the user list.

![User Created](screenshots/user-created.png)

This confirms that the account has been created successfully.

---

# Disabling a User Account

Disabling an account prevents a user from signing in while retaining all account information.

Common reasons for disabling an account include:

- Employee departure
- Temporary leave
- Security investigations
- Access suspension

## Navigation

Users → Helpdesk User → Properties

Locate:

accountEnabled

Clear the checkbox and save the changes.

![Disable Account Setting](screenshots/disable-account-setting.png)

---

# Verifying Account Disablement

After saving the changes, return to the user overview page.

Verify that:

Account Status = Disabled

![User Account Disabled](screenshots/user-account-disabled.png)

This confirms that sign-in has been blocked successfully.

---

# Enabling a User Account

To restore user access:

Users → Helpdesk User → Properties

Locate:

accountEnabled

Enable the account and save the changes.

![Enable Account Setting](screenshots/enable-account-setting.png)

---

# Verifying Account Enablement

Return to the user overview page.

Verify that:

Account Status = Enabled

![User Account Enabled](screenshots/user-account-enabled.png)

This confirms that the user can sign in again.

---

# Deleting a User Account

Deleting a user account is commonly performed during offboarding procedures.

## Navigation

Users → Helpdesk User → Delete User

Review the confirmation window before proceeding.

![Delete User Confirmation](screenshots/delete-user-confirmation.png)

Confirm the deletion.

---

# Verifying User Deletion

Navigate to:

Identity → Users → Deleted Users

Verify that Helpdesk User no longer appears within Active Users.

![User Deleted](screenshots/user-deleted.png)

---

# Reviewing Deleted Users

Deleted accounts remain available for restoration for a limited period.

Navigate to:

Identity → Users → Deleted Users

Locate Helpdesk User within the Deleted Users container.

![Deleted Users List](screenshots/deleted-users-list.png)

---

# Restoring a Deleted User

Select the account and choose:

Restore Users

![Restore User](screenshots/restore-user.png)

Review the confirmation window before proceeding.

![Restore User Confirmation](screenshots/restore-user-confirmation.png)

Select OK.

---

# Verifying User Restoration

Navigate to:

Identity → Users → All Users

Verify that Helpdesk User appears again within the active user list.

![User Restored](screenshots/user-restored.png)

This confirms that the restoration process was successful.

---

# Administrative Best Practices

When managing user accounts:

- Follow the principle of least privilege
- Verify user information before account creation
- Document administrative changes
- Disable accounts before permanent deletion when appropriate
- Confirm user identity before performing account-related actions
- Regularly review deleted accounts

---

# Key Learnings

This chapter demonstrated:

- User account creation
- User property management
- Account enablement and disablement
- User deletion procedures
- User restoration procedures
- User lifecycle administration

These are common tasks performed within IT Support and Service Desk environments.

---

# Skills Developed

By completing this chapter, the following skills were developed:

- User Administration
- Identity Management
- User Lifecycle Management
- Microsoft Entra Administration
- Service Desk Procedures
- Technical Documentation
- GitHub Documentation

---

# Chapter Summary

In this chapter, a complete user lifecycle was performed within Microsoft Entra ID.

The following tasks were completed:

- Viewed existing users
- Created a new user
- Verified user creation
- Disabled the account
- Re-enabled the account
- Deleted the account
- Restored the account

These activities represent practical administrative tasks commonly encountered in entry-level IT support and cloud administration roles.
