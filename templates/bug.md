---
type: bug

id:

status: Open

severity:

priority:

project:

module:

reported:

created:

updated:

owners:
  - AI

tags:
  - bug
---

# {{title}}

> Software Defect Documentation

---

# Summary

Provide a concise description of the defect.

Focus on the incorrect behavior rather than the implementation.

---

# Problem Statement

Describe the defect.

What is happening?

What should happen?

What is the difference?

---

# Expected Behavior

Describe the expected behavior.

Use business language whenever possible.

---

# Actual Behavior

Describe the observed behavior.

Avoid assumptions.

Document facts.

---

# Business Impact

Describe the impact.

Examples

Incorrect calculation

Financial loss

Data corruption

Workflow interruption

Security risk

Poor user experience

Operational delays

---

# Severity

Possible values

Critical

High

Medium

Low

Informational

Explain why this severity was assigned.

---

# Scope

Describe where the bug occurs.

Examples

Authentication

Payments

Registration

Reporting

Synchronization

Imports

API

UI

---

# Affected Components

List affected modules.

Examples

Authentication

OwnerService

Invoice API

Redis Cache

Angular UI

---

# Root Cause

Describe the real cause.

Explain

Why it happened

Why it was not detected earlier

Underlying architectural or business issues

Avoid superficial explanations.

---

# Reproduction Steps

Describe how to reproduce.

Example

1. Login

2. Open Property Registration

3. Add second owner

4. Save

5. Observe duplicate ownership

Reproduction should be deterministic whenever possible.

---

# Preconditions

Document required conditions.

Examples

Specific permissions

Existing records

Configuration

Feature flags

Environment

---

# Resolution

Describe the implemented solution.

Explain

What changed

Why it fixes the problem

Potential side effects

---

# Validation

Describe how the fix should be validated.

Include

Manual testing

Automated testing

Regression testing

Edge cases

Negative testing

---

# Regression Risk

Describe

Areas that may be affected

Related modules

Dependencies

Potential unintended consequences

---

# Prevention

Explain how similar bugs can be avoided.

Examples

Architecture improvements

Better validation

Additional tests

Static analysis

Monitoring

Code review improvements

---

# Related Business Rules

Reference

[[Business Rule]]

---

# Related Features

Reference

[[Feature]]

---

# Related Architecture

Reference

[[Architecture]]

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

Reference implementation history.

---

# Lessons Learned

Describe knowledge gained.

Examples

Framework behavior

Business misunderstanding

Architecture weakness

Validation gap

Infrastructure assumption

---

# Metadata

Severity

Priority

Repository

Branch

Commit

Confidence

Reported By

Resolved By

Generated At

Last Review