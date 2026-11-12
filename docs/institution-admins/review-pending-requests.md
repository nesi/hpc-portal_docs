---
title: Review pending requests
description: How organisation owners approve, reject or edit allocation orders in bulk on the REANNZ allocations page.
created_at: '2026-11-13'
tags:
- institution-admin
- allocation
---

The **REANNZ allocations** page lists every order waiting in your organisation on one screen.
You can approve or reject several at once, and edit the requested limits before you approve.

It covers orders only: new allocations, limit changes and terminations.
Project requests and end date changes still wait where
[Approving requests](approve-requests.md#find-pending-requests) says.

## Open the page

1. Log in to [https://hpc-portal.reannz.co.nz](https://hpc-portal.reannz.co.nz) with **Sign in with Tuakiri**.
2. In the sidebar, click **Quick shortcuts** next to the logo, then **Admin Review**.
   The page opens in a new tab.
3. In the page's sidebar, under **Views**, click **Pending requests**.
   The number next to it is how many requests are waiting.

You can also go straight to
[https://hpc-portal.reannz.co.nz/admin-review/#requests](https://hpc-portal.reannz.co.nz/admin-review/#requests).
Log in to the portal first. If you are not logged in, the page sends you to the login screen
and does not bring you back.

## Read the list

The tiles at the top count requests **Waiting for org owner** and **Waiting for REANNZ review**.
**Oldest request** shows how long the oldest one has waited.

Requests are listed oldest first. Each row shows:

| Column | Meaning |
| --- | --- |
| Request | The order name and who asked. Click the name to open the order in the portal. |
| Type | **Create** for a new allocation, **Update** for a limit change, **Terminate** to end one. |
| Limits and usage | Each component as current → requested, with its unit. The bar is usage; the tick is the requested limit. |
| Waiting for | **Org owner** means an owner in your organisation, such as you. **REANNZ review** means an owner has approved it. |
| Submitted | How long ago the request was made. |

Use the search box, or the **Organisation**, **Offering**, **Type** and **Waiting for** filters, to narrow the list.

The page does not refresh by itself. Reload it to see new requests.

!!! warning "Terminate requests end an allocation"
    A **Terminate** request shows its limits as **removed**.
    Approving it ends the allocation.

## Approve or reject

1. Tick the requests you want. Rows waiting for **Org owner** have a checkbox.
   To act on one request, use the **Approve** or **Reject** button on its row instead.
2. In the bar that appears, click **Approve** or **Reject**.
3. Check the dialog:
    - **Approve** shows the total requested for each component, for example compute in RSU.
    - **Reject** needs a comment saying why. The same comment goes with every selected request.
4. Click **Approve** or **Reject** to confirm.

Each row then shows **Approved** or **Rejected**.
An approved request moves to **REANNZ review**.
REANNZ then reviews it and makes recommendations if need be.

If a row shows **Already changed elsewhere; refreshed.**,
someone else acted on it first. Nothing more is needed.

!!! note "Tell the project manager when you reject"
    The portal does not email the project manager when you reject an order.
    Tell them directly, with the reason.

## Edit limits before you approve

You can change the requested limits while a request is waiting for you.

1. On the row, click **Edit limits…**.
2. Each component shows the current and requested values. Enter the new value.
   It must be zero or more, and within the offering's minimum and maximum.
3. Add a **Comment** saying why, if you wish.
4. Click **Save**.

Saving changes the request. It does not approve it.
Approve it afterwards as above.

The row shows **Edited once** or **Edited N×**. Click it to see who changed what, when, and why.
The change and your comment are kept on the order in the portal.

Once you approve a request, you can no longer edit it.

## Further reading

- To approve orders one at a time in the portal, see [Approve an order](approve-requests.md#approve-an-order).
- To watch usage across your organisation, see [Monitor allocation usage](allocation-usage.md).
