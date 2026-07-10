---
type: feature

id:

status: Active

project:

module:

priority:

created:

updated:

owners:
  - AI

tags:
  - feature
---

# {{title}}

> Feature Documentation

---

# Purpose

Describe the feature.

Answer:

What does this feature do?

Who uses it?

Why does it exist?

Avoid implementation details.

---

# Business Context

Explain the business process.

Who requested it?

Which business process depends on it?

What problem does it solve?

---

# Functional Overview

Describe the behavior from the user's perspective.

Focus on expected behavior.

Avoid technical implementation.

---

# User Flow

Describe the complete workflow.

Example

1. User opens the registration screen.

2. User fills the required fields.

3. Validation is executed.

4. Data is persisted.

5. Confirmation is displayed.

Alternative flows should be documented separately.

---

# Actors

List every actor.

Examples

Administrator

Citizen

Operator

API Client

Background Job

Integration

---

# Permissions

Describe who may execute the feature.

Reference authorization documentation whenever possible.

---

# Inputs

Document

User input

API payload

Events

Files

Imports

Parameters

Required fields

Optional fields

---

# Outputs

Describe

Responses

Generated entities

Events

Notifications

Reports

Files

Side effects

---

# Validations

Describe every important validation.

Examples

Required fields

Business validations

Authorization

Duplicate detection

State validation

Ownership validation

---

# Business Rules

Reference all related business rules.

Examples

[[Owner Validation]]

[[Invoice Lifecycle]]

[[Password Policy]]

---

# Architecture

Reference affected architecture.

Examples

[[Authentication]]

[[Payments]]

[[Properties]]

---

# Integrations

Reference external systems.

Examples

[[Stripe]]

[[RabbitMQ]]

[[Google Maps]]

[[Cloudflare]]

---

# Infrastructure

Reference infrastructure.

Examples

[[Redis]]

[[Docker]]

[[PostgreSQL]]

---

# Related ADR

Reference important decisions.

Examples

[[ADR-004 Cache]]

[[ADR-006 JWT]]

---

# Related Handoffs

Reference implementation history.

Examples

[[2026-07-10 Owner Registration]]

[[2026-08-12 Validation Refactor]]

---

# Edge Cases

Document uncommon situations.

Examples

Duplicate records

Expired sessions

Deleted users

Partial failures

Network interruption

Legacy data

---

# Error Handling

Describe

Validation errors

Business errors

Infrastructure failures

Integration failures

Retry behavior

Rollback behavior

---

# Performance Considerations

Describe

Expected load

Caching

Indexes

Pagination

Async processing

Known bottlenecks

---

# Security Considerations

Describe

Authentication

Authorization

Audit

Sensitive data

Encryption

Rate limiting

Permissions

---

# Monitoring

Describe

Metrics

Logs

Alerts

Dashboards

Health checks

Tracing

---

# Known Limitations

Describe

Current limitations

Technical debt

Framework limitations

Business constraints

Operational limitations

---

# Future Improvements

Document ideas that could improve the feature.

Avoid implementation tasks.

Describe desired evolution.

---

# Related Documentation

[[Architecture]]

[[Business]]

[[Infrastructure]]

[[Troubleshooting]]

[[ADR]]

---

# Metadata

Feature Owner

Repository

Branch

Commit

Confidence

Last Review

Generated At