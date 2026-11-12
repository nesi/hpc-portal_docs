---
title: Monitor allocations with the API
description: How institution admins use the HPC Portal API to watch allocations and end dates.
created_at: '2026-11-13'
tags:
- institution-admin
- allocation
---

!!! warning "Not yet available to organisation owners"
    The HPC Portal does not give organisation owners an API token at present.
    The steps below show how monitoring works once it does.
    Until then, use the portal: open your organisation's **Resources**
    and check the allocations with the nearest **Termination date**.

The HPC Portal has a REST API at `https://hpc-portal.reannz.co.nz/api/`.
As an organisation owner, you can use it to list your organisation's allocations,
their limits, their usage and their end dates.
The API shows you the same data as the portal does.

## Get an API token

Each call needs an API token.
The portal does not show one to organisation owners at present.
If you need API access,
[contact our Support Team](mailto:support@nesi.org.nz?subject=HPC%20Portal%20API%20access).

Send the token in the `Authorization` header of each request:

```http
Authorization: Token <your-token>
```

## List allocations ending soon

First, find your organisation's UUID:

```sh
curl -s -H "Authorization: Token $HPC_PORTAL_TOKEN" \
  "https://hpc-portal.reannz.co.nz/api/customers/?field=uuid&field=name"
```

Then list its active allocations, the soonest end date first:

```sh
curl -s -H "Authorization: Token $HPC_PORTAL_TOKEN" \
  "https://hpc-portal.reannz.co.nz/api/marketplace-resources/?customer_uuid=<org-uuid>&state=OK&o=end_date&field=name&field=project_name&field=offering_name&field=end_date&field=limits&field=current_usages"
```

Each allocation comes back like this:

```json
{
  "name": "abc01234",
  "project_name": "Example research project",
  "offering_name": "Mahuika",
  "end_date": "2026-12-01",
  "limits": {"cpu": 1000, "storage_project": 2, "storage_scratch": 10},
  "current_usages": {"cpu": 120.5, "storage_project": 0.8, "storage_scratch": 0.0}
}
```

| Parameter | Effect |
| --- | --- |
| `customer_uuid` | Only allocations in your organisation. |
| `state=OK` | Only active allocations. Repeat `state` to add others, for example `state=Updating`. |
| `o=end_date` | Soonest end date first. Use `o=-end_date` for latest first. |
| `field` | Return only the named fields. Leave it out to get every field. |

The API has no end date range filter.
Sort by `end_date` and stop reading once the dates are far enough away.
Results come in pages. Add `page_size=100` and follow the `Link` header for the next page.

For an allocation close to its end date, ask its project manager to request an extension.
See [Extending a request](../project-leads/extend-request.md).

## Keep your token safe

- Treat the token like a password. Anyone who has it can act as you in the portal.
- Keep it in an environment variable or a secret store, not in a script or a Git repository.
- Do not share it, even with colleagues. Each person needs their own.
- If you think it has leaked,
  [contact our Support Team](mailto:support@nesi.org.nz?subject=HPC%20Portal%20API%20token) at once.

The HPC Portal is built on Waldur. Its
[API documentation](https://docs.waldur.com/latest/integrator-guide/APIs/api/) covers the API in more depth.
Some endpoints are not available to organisation owners.
