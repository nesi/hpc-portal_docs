---
title: Monitor allocation usage
description: How organisation owners see which allocations in their organisation are near or over their limits and export the list.
created_at: '2026-11-13'
tags:
- institution-admin
- allocation
---

The **REANNZ allocations** page shows every active allocation in your organisation,
with usage against each limit and the end date.
Use it to spot allocations that are close to full or about to end.

## Open the page

1. Log in to [https://hpc-portal.reannz.co.nz](https://hpc-portal.reannz.co.nz) with **Sign in with Tuakiri**.
2. In the sidebar, click **Quick shortcuts** next to the logo, then **Admin Review**.
   The page opens in a new tab on **Resource allocation usage**.

You can also go straight to
[https://hpc-portal.reannz.co.nz/admin-review/](https://hpc-portal.reannz.co.nz/admin-review/).
Log in to the portal first. If you are not logged in, the page sends you to the login screen
and does not bring you back.

## Read the usage view

The tiles at the top count **Allocations**, those **At or above 80%** of a limit, and those **Over limit**.

The table lists active allocations, the fullest first.

| Column | Meaning |
| --- | --- |
| Allocation | The resource. Click it to open it in the portal. |
| Project | The project that holds it. |
| Offering | For example **Mahuika** or **Freezer**. |
| Usage vs limit | Usage against each limit, with its unit. |
| Status | The highest percentage across the components. |
| End date | When the allocation ends. |

To narrow the list:

- pick **Mahuika** or **Freezer** under **Allocations** in the page's sidebar;
- switch between **All**, **At or above 80%** and **Over limit**;
- type in the search box, or filter the **Organisation** and **Offering** columns;
- click a column header to sort, for example by **End date**.

## Act on what you find

- **Near or over a limit.** Ask the project manager whether they need more.
  They raise a limit change, and it comes to you.
  See [Review pending requests](review-pending-requests.md).
- **End date close.** Ask the project manager to request a new end date.
  See [Extending a request](../project-managers/extend-request.md).

## Export the list

Click **Export CSV**.
The file holds the rows the table shows, with each component's usage and limit,
the end date, and the project managers' email addresses.

The file contains personal data. Store and share it with care.
An email cell reads **(not visible)** when you cannot see that project's team.
