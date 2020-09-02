---
layout: post
title: Create CRM Unlicensed (Non-Interactive) User
---

# Non-Interactive User
The *non-interactive* user is not a ‘user’ in the typical sense – it is not a person but an access mode that is created with a user account. It is used for programmatic access to and from Microsoft Dynamics 365 between applications. Creating a non-interactive user account lets these applications or tools, such as a Dynamics 365 to ERP connector, authenticate and access Dynamics 365 (online), without requiring a Dynamics 365 (online) license.

# How to Create
1. Go to Office 365 Admin Center (via Dynamics 365 online Apps panel, or https://portal.office365.com)
2. Users => Active users => Add a user
3. Manage Group of the user. Add the user to the Group for the Dynamics 365.
4. Licensed the user. As the user is unlicensed user for Dynamics 365, there's no need to assign it the Dynamics 365 license. But in order for the user able to appear in the CRM, you need to assign it the Micorsoft Teams Exploratory license.
5. Wait for the user appears in CRM. This will take a while.
6. When you can see the user in CRM, open it in form and change the Access Mode from 'Read-write' to 'Non-interactive'.
7. Assign the proper Role(s) to the user as normal user. This is to assign the user the data access privilege.
