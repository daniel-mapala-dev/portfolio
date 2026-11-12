# Turning Point POS

**Year:** 2025
**Role:** Developer
**Status:** Complete

---

## The problem

A retail operation needed point-of-sale and stock control software that
matched its actual workflow rather than forcing the workflow to match
generic software.

## The solution

A point-of-sale system covering:

- Sales transaction processing
- Stock level tracking and adjustment
- Product and price management
- Daily sales reporting
- User access control

## My role

Full development: requirements, database design, application
development, and testing.

## Architecture

| Layer | Technology |
| :--- | :--- |
| Application | PHP |
| Database | MySQL |
| Frontend | HTML, CSS, JavaScript |

## Design decisions

**Transaction integrity.** Stock levels and sales records are updated
together within a transaction, so a failed sale cannot leave stock
inconsistent.

**Simplicity at the counter.** The sales interface prioritises speed of
entry, because counter staff cannot spend time navigating.

## What this demonstrates

Transactional integrity · inventory logic · reporting · practical
interface design for operational users.

## Code availability

Repository: private. Walkthrough available on request.
