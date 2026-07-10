# Engineering Memory
## Detection Rules

Version: 1.0.0

---

# Purpose

Before documenting any implementation, understand the project.

Documentation quality depends directly on understanding the repository.

Never rely solely on the current conversation.

The repository is the primary source of truth.

---

# Detection Priority

Always inspect information in the following order.

1. Repository structure

2. Build files

3. Dependency files

4. Configuration files

5. Git metadata

6. Existing documentation

7. Conversation

The conversation is supplementary.

Never use it as the only source.

---

# Repository Identity

Determine:

Project Name

Repository Name

Repository URL

Default Branch

Current Branch

Current Commit

Workspace Root

Repository Type

Confidence

---

# Repository Type

Determine whether the project is:

Single Repository

Monorepo

Workspace

Multi-module

Library

CLI

Backend

Frontend

Fullstack

Infrastructure

Unknown

Never guess.

---

# Programming Languages

Detect every language.

Examples

Java

Kotlin

TypeScript

JavaScript

Python

Go

Rust

C#

PHP

Ruby

Swift

Dart

C++

SQL

Shell

YAML

Markdown

---

# Package Managers

Detect automatically.

Examples

npm

pnpm

bun

yarn

Maven

Gradle

Cargo

Go Modules

Composer

NuGet

Pip

Poetry

---

# Frameworks

Detect frameworks.

Examples

Spring Boot

Spring MVC

Hibernate

JPA

Angular

React

Next.js

Vue

Nuxt

NestJS

Express

Fastify

Laravel

Django

Flask

ASP.NET

Quarkus

Micronaut

Gin

Fiber

Echo

Never assume.

---

# Infrastructure

Detect infrastructure.

Examples

Docker

Docker Compose

Kubernetes

Helm

Terraform

Ansible

Traefik

Nginx

Apache

Coolify

GitHub Actions

GitLab CI

Jenkins

ArgoCD

Prometheus

Grafana

Loki

Tempo

OpenTelemetry

---

# Databases

Detect all databases.

Examples

PostgreSQL

MySQL

MariaDB

SQL Server

Oracle

SQLite

MongoDB

Redis

ElasticSearch

OpenSearch

Cassandra

Neo4j

DynamoDB

InfluxDB

---

# Messaging

Detect messaging systems.

RabbitMQ

Kafka

ActiveMQ

Redis Streams

Amazon SQS

Google Pub/Sub

Azure Service Bus

NATS

---

# Cloud

Detect cloud providers.

AWS

Azure

Google Cloud

Cloudflare

DigitalOcean

Hetzner

Oracle Cloud

Render

Railway

Fly.io

Vercel

Netlify

---

# Repository Structure

Understand:

Modules

Packages

Services

Applications

Libraries

Shared code

Utilities

Configuration

Tests

Documentation

Assets

---

# Architecture

Infer architecture.

Examples

Layered

Hexagonal

Clean Architecture

DDD

Microservices

Monolith

Modular Monolith

Serverless

Event Driven

CQRS

Unknown

Confidence must always be recorded.

---

# Git Analysis

Inspect:

Current Branch

Commit

Modified Files

Deleted Files

Added Files

Renamed Files

Staged Files

Untracked Files

Recent History

Never depend exclusively on Git history.

---

# Existing Documentation

Read existing documentation before generating new documentation.

Prioritize:

README

Architecture

ADR

Business Rules

Troubleshooting

INDEX

Recent Handoffs

Never overwrite established knowledge without reason.

---

# Build System

Determine how the project is built.

Examples

Maven

Gradle

TurboRepo

Nx

Webpack

Vite

Rollup

Bazel

Make

Taskfile

Cargo

---

# Testing

Detect testing frameworks.

JUnit

Mockito

Vitest

Jest

Playwright

Cypress

Testcontainers

JUnit5

PyTest

Go Test

---

# Deployment

Identify deployment technologies.

Docker

Compose

Helm

Kubernetes

Cloud Run

Lambda

Coolify

Vercel

Netlify

Render

Railway

Fly

---

# Confidence Levels

Every automatic detection must have confidence.

High

Information explicitly found.

Medium

Strong evidence.

Low

Inference.

Unknown

Not enough information.

Never convert assumptions into facts.

---

# Missing Information

When something cannot be detected:

Record it.

Never invent.

Never hallucinate.

---

# Detection Quality Checklist

Repository identified

Project identified

Stack identified

Framework identified

Infrastructure identified

Architecture inferred

Documentation consulted

Confidence assigned

Unknown items recorded

---

# Golden Rule

Understand first.

Document second.

Never reverse this order.