# Engineering Memory
## Quality Rules

Version: 1.0.0

---

# Purpose

Documentation is part of the implementation.

Poor documentation creates future technical debt.

Before storing any knowledge, evaluate its quality.

The objective is not to maximize the amount of documentation.

The objective is to maximize usefulness.

---

# Documentation Philosophy

Good documentation answers questions.

Great documentation prevents questions.

Always optimize for future understanding.

Imagine an engineer reading this documentation one year from now.

Will they understand why the decision was made?

If not,

improve the documentation.

---

# Definition of Done

A development task is only complete when:

✓ Code is implemented.

✓ Tests have been executed when applicable.

✓ Documentation has been updated.

✓ Knowledge has been extracted.

✓ Existing notes have been updated.

✓ Duplicate documentation has been avoided.

Only then is the task complete.

---

# Engineering Questions

Every document should answer as many of these questions as possible.

What changed?

Why was it necessary?

How does it work?

What assumptions exist?

Which trade-offs were made?

Which alternatives were rejected?

Which risks remain?

How can it be tested?

What should another engineer know?

---

# Explain Why

Never stop at describing what happened.

Always explain why.

Bad

"Redis was added."

Good

"Redis was introduced to reduce repeated database access for frequently requested reference data. Local in-memory caching was rejected because multiple application instances require shared cache consistency."

Reasoning is more valuable than implementation details.

---

# Technical Decisions

Every significant decision should include

Decision

Motivation

Alternatives

Trade-offs

Consequences

Future implications

If these cannot be explained,

the decision has not been documented properly.

---

# Avoid Low-Value Documentation

Do not write documentation that merely repeats code.

Bad

"The UserService contains methods."

Good

"The UserService centralizes permission validation to avoid duplicated authorization logic across controllers."

Documentation should explain intent.

Code already explains syntax.

---

# Explain Assumptions

Whenever assumptions exist,

document them.

Examples

Expected database constraints

Expected API behavior

Expected deployment topology

Framework limitations

Performance assumptions

Security assumptions

Hidden assumptions create future bugs.

---

# Unknown Information

It is acceptable to document uncertainty.

Example

"The deployment strategy could not be determined automatically."

Never invent missing information.

---

# Context Preservation

Future engineers should not require access to:

Chat history

Pull Requests

Meetings

Slack

Email

Everything necessary should already exist inside the knowledge base.

---

# Conciseness

Documentation should be concise.

Remove repetition.

Remove filler.

Remove obvious statements.

Keep explanations complete.

Avoid unnecessary verbosity.

---

# Technical Accuracy

Accuracy is more important than completeness.

Incomplete but correct documentation is better than complete but incorrect documentation.

Never speculate.

---

# Knowledge Reuse

Before writing:

Search existing documentation.

If equivalent knowledge exists:

Update it.

Do not duplicate it.

Knowledge should evolve.

Not multiply.

---

# Examples

Whenever a concept is difficult,

include an example.

Examples dramatically improve comprehension.

Prefer practical examples over theoretical explanations.

---

# Audience

Write for

Engineers

Architects

Future AI Agents

Assume technical readers.

Do not oversimplify.

---

# Language

Be objective.

Avoid marketing language.

Avoid opinions.

Avoid unnecessary adjectives.

Prefer precise technical language.

---

# Confidence

Every inferred statement should include confidence.

High

Medium

Low

Unknown

Never present assumptions as facts.

---

# Documentation Score

Before saving documentation,

evaluate the following categories.

Architecture

★★★★★

Business Rules

★★★★★

Implementation

★★★★★

Technical Decisions

★★★★★

Validation

★★★★★

Troubleshooting

★★★★★

Infrastructure

★★★★★

Knowledge Reuse

★★★★★

Links

★★★★★

Completeness

★★★★★

Categories with low quality should be improved before saving.

---

# Self Review

Before finishing,

review the documentation.

Ask yourself

Would another engineer understand this?

Would another AI continue the work?

Would I understand this in one year?

If the answer is "No",

continue improving.

---

# Completion Checklist

Repository understood

Task understood

Architecture impact documented

Business impact documented

Technical decisions documented

Risks documented

Validation documented

Knowledge extracted

Existing notes updated

Duplicate notes avoided

Wiki links created

Metadata included

Confidence recorded

Quality reviewed

---

# Golden Rule

The objective is not to document everything.

The objective is to preserve understanding.

Understanding outlives implementation.

Code changes.

Knowledge remains.