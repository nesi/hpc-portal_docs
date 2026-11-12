---
title: Check allocation usage
description: How project managers see usage against limits for all their allocations, and which of their requests are still waiting.
created_at: '2026-11-13'
tags:
- project-manager
- allocation
---

The **REANNZ allocations** page shows all your allocations on one screen,
with usage against each limit and the end date.
It also shows which of your requests are still waiting, and for whom.

The page is read-only for project managers.
To change anything, use the resource in the portal.

## Open the page

1. Log in to [https://hpc-portal.reannz.co.nz](https://hpc-portal.reannz.co.nz) with **Sign in with Tuakiri**.
2. In the sidebar, click **Quick shortcuts** next to the logo, then **Admin Review**.
   The page opens in a new tab.

You can also go straight to
[https://hpc-portal.reannz.co.nz/admin-review/](https://hpc-portal.reannz.co.nz/admin-review/).
Log in to the portal first. If you are not logged in, the page sends you to the login screen
and does not bring you back.

## See usage against limits

Under **Views**, click **Resource allocation usage**.
The table lists your active allocations, the fullest first.

- **Usage vs limit** shows usage against each limit, with its unit.
- **Status** shows the highest percentage across the components.
- **End date** shows when the allocation ends.

The tiles count allocations **At or above 80%** of a limit and **Over limit**.
Click **Export CSV** to download the list.

When an allocation nears a limit, ask for more.
See [Change allocation limits](change-limits.md).
When its end date is close, ask for a new one.
See [Extending a request](extend-request.md).

## See your waiting requests

Under **Views**, click **Pending requests**.
The list shows your new allocations and limit changes that are not done yet, oldest first.

| Waiting for | Meaning |
| --- | --- |
| Org owner | An organisation owner at your institution has not approved it yet. |
| REANNZ review | Your institution approved it. REANNZ is reviewing it. |

**Limits and usage** shows each component as current → requested.
If an owner changed your request before approving it, the row shows **Edited once** or **Edited N×**.
Click it to see what changed and why.

A request that leaves this list is done or was declined.
Open the resource to check. See [Track an order](track-order.md).
