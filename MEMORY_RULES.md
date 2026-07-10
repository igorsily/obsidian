# Engineering Memory
## Memory Rules

Version: 1.0.0

---

# Purpose

Not every piece of information deserves permanent storage.

The purpose of these rules is to ensure that only valuable engineering knowledge becomes part of the project's long-term memory.

The knowledge base should become more useful over time, not larger.

Always optimize for signal over noise.

---

# Memory Philosophy

Think like an experienced software engineer.

Ask yourself:

"If I return to this project in one year, would I be glad this information was documented?"

If the answer is no,

do not store it.

---

# Long-Term Knowledge

The following information should almost always be preserved.

## Architecture

Examples

System boundaries

Modules

Services

Data flow

Authentication

Caching

Messaging

Persistence

Infrastructure

API design

Dependency relationships

Deployment model

---

## Business Rules

Document business knowledge.

Examples

Who may perform an action.

Validation rules.

State transitions.

Domain constraints.

Financial calculations.

Permission rules.

Lifecycle rules.

Never assume these rules are obvious.

---

## Technical Decisions

Document every meaningful decision.

Include:

Decision

Reason

Alternatives

Trade-offs

Consequences

Future engineers should understand why the decision exists.

---

## Infrastructure Knowledge

Preserve knowledge about

Docker

Kubernetes

Networking

Cloud

CI/CD

Redis

RabbitMQ

Databases

Reverse proxies

Storage

Secrets

Monitoring

Logging

---

## Framework Knowledge

Capture project-specific framework knowledge.

Examples

Spring Boot conventions

Angular architecture

React patterns

Next.js limitations

Hibernate behavior

MapLibre configuration

Avoid copying official documentation.

Only preserve knowledge discovered inside the project.

---

## Troubleshooting

Preserve operational knowledge.

Document:

Symptoms

Diagnosis

Root Cause

Resolution

Prevention

This knowledge becomes extremely valuable over time.

---

## Performance

Document performance discoveries.

Examples

Expensive queries.

Caching strategies.

Memory leaks.

Thread bottlenecks.

Network latency.

Large payloads.

Optimization decisions.

---

## Security

Document security decisions.

Authentication.

Authorization.

Encryption.

Secrets.

Rate limiting.

Audit logging.

Never expose secrets.

---

## Integrations

Document external integrations.

Include

Purpose

Authentication

Limitations

Failure modes

Dependencies

---

# Temporary Knowledge

Some information should not become permanent.

Examples

Today's discussion.

Temporary implementation ideas.

Brainstorming.

Drafts.

Work in progress.

Half-finished experiments.

Meeting notes.

Personal reminders.

Keep temporary information outside the permanent knowledge base.

---

# Do Not Store

Never preserve:

Random console output

Build logs

Temporary errors

Debug sessions

Stack traces without analysis

Generated files

Personal opinions

Conversation transcripts

Repeated information

Noise

---

# Learning

Whenever something unexpected is discovered:

Ask:

"Will another engineer eventually encounter this?"

If yes,

document it.

Otherwise,

discard it.

---

# Duplicate Detection

Before creating knowledge:

Search existing documentation.

If an equivalent concept already exists:

Update it.

Do not duplicate it.

Knowledge should evolve,

not multiply.

---

# Knowledge Lifecycle

Every piece of knowledge has one of four states.

## Active

Current and accurate.

## Updated

Existing knowledge improved.

## Deprecated

Still useful for historical context.

## Archived

No longer relevant.

Never delete historical engineering knowledge without explicit instruction.

---

# Confidence

When documenting inferred knowledge,

indicate confidence.

Example

High

Medium

Low

Do not present assumptions as facts.

---

# Completeness

Perfect documentation is not required.

Useful documentation is.

If only part of the knowledge is available,

document what is known.

Clearly identify unknown areas.

---

# Memory Checklist

Before saving information ask:

Is this useful in six months?

Does it explain a decision?

Does it explain a business rule?

Does it explain architecture?

Does it explain infrastructure?

Does it prevent future mistakes?

Does it help another engineer?

If most answers are "No",

do not store it.

---

# Golden Rule

Store knowledge.

Not conversations.

Store reasoning.

Not chat history.

Store understanding.

Not raw information.

The purpose of Engineering Memory is to preserve engineering intelligence,

not conversation transcripts.