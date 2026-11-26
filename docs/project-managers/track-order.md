---
title: Track an order
description: How project managers check the status of an order and know when a resource is ready.
created_at: '2026-11-13'
tags:
- how-to
- project-manager
- allocation
---

A new allocation and a limit change are both orders.
Each order goes to an organisation owner at your institution for approval,
then REANNZ reviews it and makes recommendations if need be.

This page is for project managers.
Project members cannot see orders; ask your project manager.

## Find your orders

The portal has no orders tab on the project. Use one of these instead.

**All your orders.**

1. Click **REANNZ Marketplace** in the sidebar.
2. Click the **Orders** tab.
3. To see one project only, filter by **Project**.

**Waiting requests at a glance.**
The **Pending requests** view on the REANNZ allocations page shows who each request is waiting for.
See [Check allocation usage](allocation-usage.md#see-your-waiting-requests).

**Orders for one resource.**

1. Open the resource: go to **Projects**, open your project, click the **Resources** tab and select the allocation.
2. Click the **Resource metadata** tab, then **Order history**.

## Order states

| State | Meaning |
| --- | --- |
| Pending consumer approval | Waiting for an organisation owner at your institution. |
| Pending provider approval | Approved by your institution. REANNZ is reviewing it. |
| Pending start date | Approved by your institution and REANNZ. Waiting for the start date you chose. |
| Executing | The change is being applied. |
| Done | The change is in place. |
| Rejected | Declined. The portal does not email you; ask your organisation owner why. |
| Canceled | Withdrawn. Nothing changed. |
| Erred | Something went wrong. [Contact our Support Team](mailto:support@nesi.org.nz?subject=HPC%20Portal%20Request) or [raise a support request](../getting-started/get-help.md). Quote your project code and allocation name. |

If an order waits too long for your institution,
ask an organisation owner there to check it.
They approve orders as described in [Approve an order](../access-enablers/approve-requests.md#approve-an-order).

## Choose a start date

When you order a new allocation, the **Start date** field under **Final configuration** is optional.

**No start date.**
Setup starts as soon as REANNZ finishes its review.

**With a start date.**
The order still needs both approvals first.
Once approved, it shows **Pending start date** until that date.
Setup then starts automatically. You do not need to do anything.

- The earliest start date is tomorrow.
  It cannot be after your project's end date.
- The portal counts dates in UTC and checks every two hours.
  Setup starts on the start date from about 1 pm in summer (NZDT) or midday in winter (NZST).
- If approval comes after the start date, setup starts as soon as REANNZ finishes its review.
- While the order waits, the new resource already shows **Creating**.
  This does not mean setup has started. Check the order state.
- You cannot change the start date after you submit the order.
  To change it, [contact our Support Team](mailto:support@nesi.org.nz?subject=HPC%20Portal%20start%20date).
  Quote your project code and allocation name.

## When the resource is ready

The portal does not email you when REANNZ finishes its review or marks the order done.
Check the resource instead.

| Resource state | Meaning |
| --- | --- |
| Creating | A new allocation is being set up, or is waiting for its start date. |
| Updating | A limit change is being applied. |
| OK | The allocation is ready, with the limits shown. |
| Erred | Something went wrong. Contact our Support Team. |

When a new allocation shows **OK**, your team can use it.
Point them to [Access Mahuika](../members/access-mahuika.md).
