# HRD Portal — Secure Collaboration Platform

**Client:** Delivered with UNDP support
**Year:** 2025
**Role:** Designer and implementer
**Status:** In production

---

## The problem

Human rights defenders in Malawi needed to share resources and
communicate securely. Standard collaboration tools assume a threat model
that does not match their situation: they assume the platform operator,
the network, and the account provider are all trusted. For this user
group, none of those assumptions hold safely.

## The solution

A purpose-built collaboration platform with security designed for a
high-risk user population:

- Encrypted storage of shared resources
- Strict access control with explicit sharing permissions
- Audit logging of access and changes
- Minimal data collection by design
- Controlled account provisioning

## My role

Design and implementation, including the security model, access control
design, encryption approach, and deployment.

## Architecture

| Layer | Technology |
| :--- | :--- |
| Application | PHP |
| Supporting services | Python |
| Security | Encryption at rest, RBAC, audit logging |
| Access model | Explicit per-resource sharing permissions |

## Design decisions

**Least privilege as the default.** Users see nothing until a resource is
explicitly shared with them. There is no organisation-wide visibility
tier, because in this context a broad visibility tier is the vulnerability.

**Explicit sharing over role inheritance.** Sharing is granted per user
per resource, with revocation that takes effect immediately, rather than
inherited through group membership.

**Audit everything.** Every access, share, and change is logged. Members
of a high-risk group need to know who has seen what.

**Minimal collection.** The platform stores only what is needed to
operate. Data that is not collected cannot be compromised.

## What this demonstrates

Security-first system design · threat modelling for a specific user
population · encryption and access control implementation · audit trail
design · understanding of data protection obligations.

## Code availability

Source code is private. The security model and design approach can be
discussed in detail on request.
