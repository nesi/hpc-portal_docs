---
title: How the HPC Portal works
created_at: '2026-11-23'
tags:
- explanation
- portal
- allocation
description: How organisations, projects, resources and orders relate in the REANNZ HPC Portal, and who approves what.
---

This page explains the ideas behind the
[REANNZ HPC Portal](https://hpc-portal.reannz.co.nz).
Read it once before you request or approve anything.
For step-by-step tasks, see the guides for your role.

## Organisations, projects and resources

The portal has three levels.

**Organisation.** Your institution.
Its organisation owners decide what projects at the institution may use.

**Project.** A piece of research.
Every project belongs to one organisation and has a team.
Each project gets a project code, for example `bsi0NNNN`.

**Resource.** An allocation the project holds on a service,
such as compute on Mahuika or storage on Freezer.
Each resource has limits and an end date, called the **Termination date**.

The services on offer are *offerings*.
You find them in the **REANNZ Marketplace**.

## Roles

A role links a person to a project or an organisation.
One person can hold several roles.

- A **project member** uses the project's resources.
- A **project manager** runs the project.
  They order resources, change limits and ask for new end dates.
- An **organisation owner** approves what projects in their organisation ask for.

Whoever requests a new project becomes its project manager.

## Orders

You do not get a resource directly.
You place an *order*, and the order is approved.

Two things are orders:

- a new resource;
- a change to the limits of an existing resource.

An order passes two checks:

1. An organisation owner at your institution approves it.
2. REANNZ reviews it and makes recommendations if need be.

The resource is ready, or the new limits apply, when REANNZ marks the order done.
The resource then shows **OK**.

An order placed by an organisation owner skips the first check.

## End dates

An end date change is not an order.
A project manager requests it, and an organisation owner approves it.
REANNZ does not review it, so the new date applies at once.

A new end date does not change limits.
To renew *and* grow an allocation, make both requests.

## Renewing is not a new project

A new project always gets a new project code.
To keep working on the same project, extend the end date of its resources.
Do not request a new project.

## How new projects start

There are three routes:

- a **group invitation link** that your organisation shares;
- an **organisation owner** creates the project for you;
- a **call for proposals**, if your organisation runs one.

A new project has no resources.
Its project manager orders them, unless a call proposal ordered them already.

## What the portal tells you, and what it does not

The portal emails organisation owners when a request needs them.
It emails a reminder 7 days and 1 day before an end date.

It does **not** email you when:

- REANNZ finishes its review;
- an order is done;
- an order is declined.

Check the resource in the portal for the result.

## Where to go next

- [Tour the HPC Portal](portal-overview.md), if you have not yet.
- [Portal reference](portal-reference.md), to look up roles and screens.
- Your guides: [project members](../members/index.md),
  [project leads](../project-leads/index.md),
  [institution admins](../institution-admins/index.md).

The HPC Portal is built on Waldur.
The [Waldur user guide](https://docs.waldur.com/latest/user-guide/) covers these ideas in more depth.
Some screens may differ from the REANNZ HPC Portal.
