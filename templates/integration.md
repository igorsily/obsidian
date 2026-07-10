---
type: integration

id:

status: Active

project:

provider:

category:

created:

updated:

owners:
  - AI

tags:
  - integration
---

# {{title}}

> External Integration Documentation

---

# Purpose

Describe the integration.

Answer:

What external system is integrated?

Why is this integration required?

Who depends on it?

---

# Overview

Provide a high-level overview.

Examples

Payment Gateway

Authentication Provider

Maps

SMS

Email

Webhook

Cloud Storage

ERP

Government API

Internal Service

---

# Business Context

Explain why this integration exists.

Examples

Receive payments

Send notifications

Authenticate users

Store files

Synchronize data

Generate invoices

Validate documents

---

# Provider Information

Document

Provider

Service

Environment

Official Documentation

Support Contact

Dashboard URL

Status Page

---

# Authentication

Describe

API Keys

OAuth

JWT

Mutual TLS

Basic Auth

Bearer Token

Certificates

Rotation strategy

Secret storage

Never expose secrets.

---

# Endpoints

Document every relevant endpoint.

Include

Purpose

HTTP Method

Authentication

Request

Response

Timeout

Retry policy

Idempotency

---

# Data Flow

Explain how data moves.

Example

User

↓

Application

↓

Validation

↓

Integration Client

↓

External API

↓

Response

↓

Persistence

↓

Notification

---

# Request Mapping

Describe

Input fields

Transformations

Validation

Serialization

Headers

Encoding

Compression

---

# Response Mapping

Describe

Returned fields

Error mapping

Status codes

Validation

Persistence

Events

---

# Failure Modes

Document expected failures.

Examples

Timeout

Authentication failure

Rate limit

Invalid payload

Unavailable service

Partial failure

Unexpected response

---

# Retry Strategy

Describe

Retry conditions

Retry intervals

Backoff strategy

Maximum attempts

Dead letter behavior

Manual intervention

---

# Error Handling

Explain

Validation errors

Network failures

Business errors

Infrastructure errors

Fallback behavior

---

# Security

Document

Authentication

Authorization

Secret storage

Token expiration

Certificate management

Encryption

Audit

---

# Performance

Document

Latency

Caching

Concurrency

Connection pooling

Rate limiting

Expected throughput

---

# Monitoring

Document

Metrics

Logs

Alerts

Dashboards

Tracing

Health checks

---

# Testing

Explain

Unit testing

Integration testing

Sandbox

Mocking

Contract testing

Load testing

Manual validation

---

# Operational Considerations

Document

Maintenance windows

Rate limits

Provider limitations

Versioning

Breaking changes

Rollback

---

# Known Limitations

Document

API limitations

Business limitations

Technical debt

Known bugs

Provider restrictions

---

# Related Features

Reference

[[Feature]]

---

# Related Architecture

Reference

[[Architecture]]

---

# Related Infrastructure

Reference

[[Infrastructure]]

---

# Related Business Rules

Reference

[[Business Rule]]

---

# Related ADR

Reference

[[ADR]]

---

# Related Troubleshooting

Reference

[[Troubleshooting]]

---

# Related Handoffs

Reference

[[Handoffs]]

---

# Metadata

Provider

Repository

Branch

Commit

Confidence

Last Review

Generated At