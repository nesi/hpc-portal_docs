---
title: Change allocation limits
description: How project leads ask for more compute (RSU) or storage (TiB) on an existing resource.
created_at: '2026-11-13'
tags:
- project-lead
- allocation
---

Each allocation has a limit for each component,
for example compute in RSU and storage in TiB.
To make an allocation bigger or smaller, change its limits.

To keep an allocation past its end date, ask for a new end date instead.
See [Extending a request](extend-request.md).

## Before you start

- You need the **Project manager** role on the project.
  Project members cannot change limits; ask your project manager.
- The allocation must already exist.
  For a new allocation, see [Order an allocation](request-new-project.md#order-an-allocation).
- Check current usage first.
  Open the resource and look at its **Usage history** chart.

## Request a limit change

1. Log in to [https://hpc-portal.reannz.co.nz](https://hpc-portal.reannz.co.nz) with **Sign in with Tuakiri**.
2. Open the resource: go to **Projects**, open your project, click the **Resources** tab and select the allocation.
3. Click **Actions**, then **Change limits**.
4. The **Change resource limits** dialog shows each component with its **Usage** and **Current limit**.
   Enter the **New limit** for each component you want to change.
5. Click **Request for a change**.

## What happens next

A limit change is an order.

1. An organisation owner at your institution approves or declines it.
2. REANNZ then reviews it and makes recommendations if need be.
3. The new limits apply when REANNZ marks the order done.

To follow its progress, see [Track an order](track-order.md).

!!! note "Check the resource for the result"
    The portal does not email you when REANNZ finishes its review or marks the order done.
    It also sends no email when an order is declined, so ask your organisation owner for the outcome.
    Open the resource. It shows **OK** with the new limits when the change is in place.

Allocations are subject to the size and duration limits in force at the time.
See [Project Extensions and New Allocations on Existing Projects](https://docs.nesi.org.nz/Getting_Started/Allocations/Allocations_and_Extensions/).
