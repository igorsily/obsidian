# Engineering Memory
## Linking Rules

Version: 1.0.0

---

# Purpose

Engineering knowledge should never exist in isolation.

Every note is part of a larger knowledge graph.

Documentation becomes exponentially more valuable when related concepts are connected.

The objective is to create a navigable engineering knowledge base rather than a collection of disconnected documents.

---

# Philosophy

Think in relationships.

Do not ask:

"What note am I writing?"

Instead ask:

"What knowledge already exists that relates to this?"

Every note should help engineers discover other relevant knowledge.

---

# Wiki Links

Always prefer Obsidian Wiki Links.

Correct

[[Authentication]]

[[Redis]]

[[Spring Boot]]

[[Payments]]

Avoid Markdown links for internal documentation whenever possible.

Wiki Links are the default.

---

# Bidirectional Thinking

Whenever creating a note ask:

Which existing notes should point here?

Which notes should this note reference?

Knowledge should be discoverable from multiple entry points.

---

# Link Existing Knowledge

Before saving a document:

Search for related documentation.

Examples

Architecture

ADR

Business Rules

Features

Infrastructure

Troubleshooting

Frameworks

Integrations

Recent Handoffs

Create links whenever relationships exist.

---

# Link Types

Every note may contain relationships.

Examples

Related Features

Related Bugs

Related ADR

Related Architecture

Related Business Rules

Related Infrastructure

Related Integrations

Related Frameworks

Related Troubleshooting

Related Handoffs

---

# Handoff Links

Every handoff should reference:

Architecture

Business Rules

ADR

Affected Features

Troubleshooting

Infrastructure

Framework Notes

Related Handoffs

Example

## Related Knowledge

[[Authentication]]

[[ADR-003 Authentication]]

[[JWT]]

[[Security]]

---

# Architecture Links

Architecture notes should reference

Business Rules

Infrastructure

Frameworks

ADR

Features

Database

API

Deployment

Never leave architecture isolated.

---

# Business Rules

Business Rules should connect to

Features

Architecture

Database

Validation

Troubleshooting

ADR

Never document business rules without showing where they apply.

---

# ADR Links

Each ADR should reference

Previous ADR

Affected Architecture

Related Infrastructure

Business Rules

Implementation Handoff

Future ADR

Architecture becomes easier to navigate when decisions are connected.

---

# Framework Notes

Framework notes should reference

Architecture

Features

Troubleshooting

Performance

Integrations

Avoid isolated framework documentation.

---

# Infrastructure

Infrastructure should reference

Deployment

Monitoring

Networking

Security

Containers

Cloud

Frameworks

Architecture

---

# Troubleshooting

Troubleshooting should reference

Affected Framework

Affected Feature

Architecture

Infrastructure

Business Rule

Known Bug

Never document a problem without linking to the affected components.

---

# Features

Features should reference

Business Rules

Architecture

Infrastructure

ADR

Related Features

Integrations

Troubleshooting

Recent Handoffs

---

# Bugs

Bug documentation should reference

Feature

Architecture

Business Rule

Troubleshooting

Root Cause

Related ADR

Never document bugs without context.

---

# README

The project README should always link to

INDEX

Architecture

ADR

Business

Infrastructure

Frameworks

Latest Handoffs

Troubleshooting

README is the project's homepage.

---

# INDEX

INDEX is the project's navigation hub.

It should link to

Recent Handoffs

Architecture

ADR

Business Rules

Features

Infrastructure

Frameworks

Releases

Troubleshooting

Integrations

README

INDEX should never become outdated.

---

# Link Density

Too few links reduce discoverability.

Too many links reduce readability.

Prefer meaningful links.

Avoid linking every technical term.

---

# Duplicate Links

Do not repeat identical links multiple times in the same section.

One meaningful reference is enough.

---

# Link Confidence

Only create links when a meaningful relationship exists.

Never force connections.

Quality is more important than quantity.

---

# Broken Links

If a note does not exist yet

Create the wiki link anyway.

Example

[[Caching]]

The note may be created later.

Broken wiki links are acceptable.

---

# Link Naming

Use concise names.

Good

[[Payments]]

[[Docker]]

[[Redis]]

[[Authentication]]

Bad

[[Complete Authentication Documentation]]

[[Docker Setup Documentation]]

---

# Navigation Sections

Whenever appropriate, end notes with

---

## Related Notes

[[Authentication]]

[[Redis]]

[[Spring Boot]]

[[ADR-002 Cache Strategy]]

[[Docker]]

---

## Related Handoffs

[[2026-07-09 Authentication Refactor]]

[[2026-08-14 JWT Improvements]]

---

## Related Business Rules

[[Password Policy]]

[[User Lifecycle]]

---

## Related Architecture

[[Authentication]]

[[Caching]]

---

This section greatly improves discoverability.

---

# Knowledge Graph

The objective is not merely documentation.

The objective is to build an engineering knowledge graph.

Every completed task should increase the connectivity of the graph.

The graph should become easier to navigate over time.

---

# Golden Rule

Never create isolated knowledge.

Every important concept should connect to the broader understanding of the project.