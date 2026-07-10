---
name: engineering-memory
version: 1.0.0
author: Igor Sily
description: AI-agnostic engineering memory framework for capturing and maintaining long-term project knowledge inside an Obsidian vault.
---

# Engineering Memory

## Mission

Your responsibility is not only to implement software.

Your responsibility is to preserve engineering knowledge.

Every completed task should leave the project easier to understand than before.

Assume every conversation will eventually disappear.

The documentation becomes the project's long-term memory.

Implementation is only complete when the relevant knowledge has been preserved.

---

# Primary Objectives

Always strive to:

- Preserve context
- Preserve reasoning
- Preserve decisions
- Preserve discoveries
- Preserve business knowledge
- Preserve architectural knowledge
- Preserve troubleshooting knowledge

Never reduce documentation to a simple summary.

---

# Default Knowledge Base

Unless explicitly instructed otherwise, the knowledge base is located at:

~/obsidian

If it does not exist:

- create it
- initialize the expected directory structure
- continue normally

Never ask the user where to save documentation unless writing to the default location fails.

---

# Repository Discovery

Before documenting anything, inspect the repository.

Determine, when possible:

- Project Name
- Repository Name
- Repository URL
- Current Branch
- Current Commit
- Monorepo or Single Repository
- Workspace Structure
- Backend Technologies
- Frontend Technologies
- Infrastructure Stack
- Build Tools
- Package Managers
- Programming Languages
- Testing Frameworks
- Deployment Strategy
- CI/CD Platform
- Architecture Style

Use every available source including:

- package.json
- README
- pom.xml
- build.gradle
- Dockerfile
- docker-compose.yml
- turbo.json
- nx.json
- Cargo.toml
- go.mod
- composer.json
- Makefile
- .git/config
- GitHub workflows
- repository structure

Never invent information.

If uncertain, explicitly record that the information could not be determined.

---

# Understand the Current Work

Before writing documentation, understand what was actually accomplished.

Use every available source:

- modified files
- git diff
- staged files
- commit message
- repository context
- current conversation

Infer:

- objective
- affected modules
- architectural impact
- business impact
- infrastructure impact

---

# Read Existing Knowledge First

Before creating any new documentation:

Read the existing knowledge stored inside the project's Obsidian folder.

Prioritize:

Project README

INDEX

Architecture

Business

Decisions

ADR

Troubleshooting

Recent Handoffs

Features

Known Bugs

Releases

The existing knowledge base is the primary source of truth.

Avoid contradicting previous documentation.

---

# Knowledge Capture

At the end of every completed task:

Capture:

## What was built

## Why it was built

## How it works

## Important assumptions

## Trade-offs

## Lessons learned

## Business knowledge discovered

## Architectural knowledge discovered

## Infrastructure knowledge discovered

## Framework limitations discovered

## Risks

## Future improvements

---

# Handoff Generation

Generate a handoff describing the completed work.

The handoff must allow another engineer to continue the project without access to previous conversations.

The handoff should explain:

Context

Objective

Implementation

Technical Decisions

Architecture Impact

Files Changed

Validation

Pending Work

Lessons Learned

Metadata

---

# Knowledge Extraction

Not everything belongs inside a handoff.

Detect reusable knowledge.

Examples:

Architecture

Business Rules

Infrastructure

Frameworks

Integrations

Deployment

Performance

Security

Database

Troubleshooting

Coding Standards

Store reusable knowledge separately.

---

# Documentation Rules

Always prefer:

Updating existing notes

instead of

Creating duplicate notes.

Never create multiple notes describing the same concept.

---

# Wiki Links

Whenever possible create Obsidian wiki links.

Example:

[[Authentication]]

[[Redis]]

[[Docker]]

[[Spring Boot]]

[[Angular]]

[[PostGIS]]

[[RabbitMQ]]

Link related notes whenever a relationship exists.

---

# Writing Style

Write for engineers.

Assume the reader joins the project six months later.

Explain reasoning.

Explain trade-offs.

Explain decisions.

Explain consequences.

Avoid generic summaries.

Capture hidden knowledge.

---

# Quality Checklist

Before considering documentation complete, verify:

✓ Repository identified

✓ Technologies identified

✓ Existing knowledge consulted

✓ Documentation updated

✓ Duplicate notes avoided

✓ Wiki links created

✓ Technical decisions documented

✓ Business rules documented

✓ Risks documented

✓ Validation documented

✓ Future work documented

---

# Completion Criteria

A task is only considered complete when:

- the implementation is finished
- the documentation is updated
- reusable knowledge has been extracted
- project memory has been preserved

Documentation is part of the implementation.

Never consider code alone to be a completed task.