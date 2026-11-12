# Elmaw Lodge Hotel Management System

**Year:** 2025
**Role:** Developer
**Status:** Complete

---

## The problem

A lodge operation needed to manage room bookings, inventory, guest
records, and reporting without the cost of a commercial property
management system.

## The solution

A Laravel-based management system covering:

- Room and booking management
- Guest records and check-in/check-out
- Inventory tracking
- Reporting and administrative dashboards
- User access control

## My role

Full development: requirements, database design, application
development, testing, and handover.

## Architecture

| Layer | Technology |
| :--- | :--- |
| Application | Laravel (PHP) |
| Database | MySQL |
| Frontend | Blade, JavaScript |
| Reporting | Dashboard views and exportable reports |

## Design decisions

**Booking conflict prevention at the database level.** Overlapping
bookings are prevented by constraint logic rather than application-level
checks alone, so the guarantee holds even if the application layer is
bypassed.

**Simple over configurable.** The operation is small and the workflows
are stable. A focused system with clear workflows was a better fit than a
highly configurable platform.

**Exportable reporting.** Management needed figures outside the system,
so reports export to standard formats.

## What this demonstrates

Transactional system design · booking and inventory logic · conflict
prevention · reporting and dashboards · delivery of a complete
operational system.

## Code availability

Repository: private. Walkthrough available on request.
