# Engineering Memory
## Project Rules

Version: 1.0.0

---

# Purpose

These rules define how project knowledge must be organized.

The objective is to create a predictable knowledge base that remains useful over months or years of development.

Every AI agent must follow the same organization.

Consistency is more important than personal preference.

---

# Default Vault

The default Obsidian Vault is:

~/obsidian

Never ask the user where the Vault is located unless writing fails.

If the Vault does not exist:

- create it
- initialize the directory structure
- continue normally

---

# Project Discovery

Every repository must map to exactly one project folder.

Example

Repository

awesome-api

becomes

~/obsidian/Projects/awesome-api/

Never create multiple project folders for the same repository.

---

# Directory Structure

Each project must follow this structure.

Projects/

    <Project>/

        README.md

        INDEX.md

        Handoffs/

        Architecture/

        ADR/

        Business/

        Decisions/

        Features/

        Bugs/

        Releases/

        Infrastructure/

        Frameworks/

        Integrations/

        Troubleshooting/

        Attachments/

Never rename these folders.

Never localize folder names.

Always use English.

---

# README

Every project must contain a README.

The README represents the current state of the project.

It should be updated over time.

It should never become a historical log.

Instead it should answer:

What is this project?

Which technologies are used?

How is it organized?

How can it be executed?

Which external systems exist?

What should a new engineer know?

---

# INDEX

Every project contains an INDEX.

The INDEX is the navigation entry point.

It links:

Recent handoffs

Architecture

ADR

Business

Features

Releases

Troubleshooting

Infrastructure

Frameworks

The INDEX should always reflect the current documentation.

---

# Handoffs

Handoffs describe completed work.

Each handoff represents one logical implementation.

Use filenames like

YYYY-MM-DD HH-mm - Task Name.md

Never overwrite a handoff.

Handoffs are immutable historical records.

---

# Architecture

Architecture notes describe long-term technical concepts.

Examples

Authentication

Caching

Messaging

Database

API

Microservices

Domain Model

Architecture notes evolve over time.

Update them.

Do not create duplicates.

---

# ADR

Architecture Decision Records document important technical decisions.

Create an ADR whenever a decision changes:

Architecture

Infrastructure

Database

Framework

Deployment

Messaging

Authentication

Caching

Storage

One ADR per decision.

---

# Business Rules

Business Rules describe domain knowledge.

Examples

Owner can have only one active property.

Invoices cannot be cancelled after payment.

Users cannot delete themselves.

Business Rules must avoid implementation details.

Describe the domain.

---

# Features

Each completed feature may receive its own documentation.

Describe:

Purpose

Behavior

Dependencies

Limitations

Future improvements

---

# Bugs

Document recurring bugs.

Include

Symptoms

Cause

Solution

Workaround

Status

Never document temporary failures.

Only recurring knowledge.

---

# Infrastructure

Infrastructure notes describe:

Docker

Kubernetes

Redis

RabbitMQ

Kafka

Cloud

Networking

Reverse Proxy

Secrets

Deployment

---

# Frameworks

Framework notes document:

Spring Boot

Angular

React

Next.js

Hibernate

JPA

MapLibre

etc.

Document only project-specific knowledge.

Avoid copying official documentation.

---

# Integrations

Document external systems.

Examples

Stripe

Google Maps

Cloudflare

AWS

Azure

SMTP

OAuth

REST APIs

---

# Troubleshooting

Document recurring operational problems.

Include

Problem

Diagnosis

Root Cause

Resolution

Prevention

---

# Attachments

Store supporting assets.

Examples

Images

Diagrams

Architecture drawings

Flowcharts

SQL files

Never store generated binaries.

---

# Naming

Prefer concise names.

Good

Authentication

Caching

Payments

Owners

Bad

Authentication Documentation Final Version

---

# Dates

Always use ISO dates.

Example

2026-07-09

Never use locale-specific formats.

---

# Links

Always create wiki links.

Example

[[Authentication]]

[[Redis]]

[[Docker]]

[[ADR-001 Authentication]]

Knowledge should become a connected graph.

---

# Ownership

Knowledge belongs to the project.

Never reference individual conversations.

Never reference temporary chat context.

Documentation should survive the disappearance of any AI session.

---

# Updating

When information changes:

Update the existing note.

Do not create another note.

Historical evolution belongs inside Git.

Not inside duplicated notes.

---

# Principle

A project should become easier to understand after every completed task.

Never leave the documentation worse than it was before.