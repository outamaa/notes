---
date: 2021-01-13T09:14
---

# Datomic

## Setting up Datomic for local dev

- [Local Dev and CI with dev-local](https://docs.datomic.com/cloud/dev-local.html)
- Download local dev tools
  - Request from above page, get link in email
  - Download, install
  - Setup your personal maven tools.deps etc settings, link also in email

## What can be retracted?

- You can retract facts that assert that an entity has an attribute
  with some value.
- You can't retract the facts that assert the existence of the
  attribute, that is you can't retract schema assertions.
