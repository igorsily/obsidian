---
type: business-rule

id:

status: Active

project:

domain:

owners:
  - AI

created:

updated:

tags:
  - business
---

# {{title}}

> Business Rule

---

# Purpose

Describe the business rule.

What does this rule enforce?

Who is affected?

Why does this rule exist?

---

# Business Context

Explain the business process.

Where does this rule apply?

Which users are involved?

Which business event triggers it?

---

# Rule Description

Describe the rule using plain language.

Avoid implementation details.

Good example

Only one active owner may exist for a property.

Bad example

Validate owner.active == true.

---

# Motivation

Explain why this rule exists.

Examples

Legal requirement

Financial rule

Operational process

Security requirement

Customer requirement

Legacy constraint

---

# Scope

Describe where the rule applies.

Examples

Registration

Authentication

Payments

Invoices

Properties

Users

Notifications

Imports

Exports

---

# Preconditions

What must be true before this rule applies?

Example

The property already exists.

The user is authenticated.

The invoice is unpaid.

---

# Rule

Describe the rule precisely.

If useful, split into steps.

Example

1. Validate ownership.

2. Check active contracts.

3. Reject duplicates.

4. Persist ownership.

---

# Exceptions

List situations where the rule does not apply.

Explain why.

---

# Validation

How should the rule be validated?

Examples

UI validation

API validation

Database constraint

Scheduled process

Background worker

---

# Error Behavior

Describe what happens when the rule is violated.

Example

HTTP 409

Validation message

Rollback

Audit log

Notification

---

# Business Impact

Describe what happens if this rule is removed or ignored.

Examples

Duplicate invoices

Invalid ownership

Financial inconsistency

Data corruption

Legal issues

---

# Dependencies

Reference related rules.

Examples

[[Property Lifecycle]]

[[Owner Validation]]

[[Authentication]]

---

# Related Features

Reference affected features.

Examples

[[Property Registration]]

[[Transfer Ownership]]

---

# Related Architecture

Examples

[[Properties]]

[[Authentication]]

[[Database]]

---

# Related ADR

Reference architecture decisions.

Examples

[[ADR-004 Ownership Model]]

---

# Related Handoffs

Reference implementation history.

Examples

[[2026-07-12 Property Ownership]]

---

# Examples

Provide practical examples.

## Valid

Property A

Owner John

Status Active

Accepted

---

## Invalid

Property A

Owner John

Owner Mary

Both Active

Rejected

---

# Edge Cases

Describe unusual situations.

Examples

Migration

Imports

Legacy data

Deleted users

Archived properties

---

# Future Considerations

Describe possible future changes.

Examples

Multiple ownership

Temporary ownership

Co-ownership

International legislation

---

# Metadata

Business Area

Repository

Branch

Commit

Confidence

Last Review

Generated At