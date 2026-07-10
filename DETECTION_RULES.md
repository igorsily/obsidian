# Engineering Memory
## Detection Rules

Version: 1.0.0

---

# Propósito

Antes de documentar qualquer implementação, entenda o projeto.

A qualidade da documentação depende diretamente do entendimento do repositório.

Nunca dependa apenas da conversa atual.

O repositório é a fonte primária da verdade.

---

# Prioridade de Detecção

Sempre inspecione a informação na seguinte ordem.

1. Estrutura do repositório

2. Arquivos de build

3. Arquivos de dependência

4. Arquivos de configuração

5. Metadados do Git

6. Documentação existente

7. Conversa

A conversa é suplementar.

Nunca a use como única fonte.

---

# Identidade do Repositório

Determine:

Nome do Projeto

Nome do Repositório

URL do Repositório

Branch Padrão

Branch Atual

Commit Atual

Raiz do Workspace

Tipo de Repositório

Confiança

---

# Resolução de Projeto

Após identificar o repositório, resolva a pasta do projeto no Obsidian.

Fluxo esperado:

1. Detectar Repositório

2. Determinar Nome do Projeto

3. Verificar

~/obsidian/Projects/<Project>

4. Existe?

5. Sim → Continuar

6. Não → Inicializar estrutura do projeto a partir de `project-template/`

7. Continuar

## Nome do Projeto

Use o nome do repositório ou o nome da pasta raiz do workspace como slug do projeto.

Exemplo

Repositório awesome-api

torna-se

~/obsidian/Projects/awesome-api/

## Inicialização do Vault

Se ~/obsidian não existir:

- crie
- crie Projects/
- crie Knowledge/
- crie Templates/
- crie Inbox/
- continue normalmente

Nunca pergunte ao usuário onde armazenar documentação.

## Inicialização do Projeto

Se ~/obsidian/Projects/<Project> não existir:

- replique o diretório `project-template/` da skill nesse path
- continue normalmente

Nunca peça confirmação.

Nunca pule a inicialização.

## Política de Monorepo

Um monorepo ou workspace mapeia para exatamente uma pasta de projeto.

Use o nome da raiz do workspace como nome do projeto.

Não crie uma pasta de projeto por package na V1.

---

# Tipo de Repositório

Determine se o projeto é:

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

Nunca chute.

---

# Linguagens de Programação

Detecte toda linguagem.

Exemplos

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

# Gerenciadores de Pacotes

Detecte automaticamente.

Exemplos

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

Detecte frameworks.

Exemplos

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

Nunca assuma.

---

# Infrastructure

Detecte infraestrutura.

Exemplos

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

Detecte todos os bancos de dados.

Exemplos

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

Detecte sistemas de mensageria.

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

Detecte provedores de cloud.

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

# Estrutura do Repositório

Entenda:

Módulos

Packages

Serviços

Aplicações

Libraries

Código compartilhado

Utilities

Configuração

Testes

Documentação

Assets

---

# Architecture

Infira a arquitetura.

Exemplos

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

A confiança deve sempre ser registrada.

---

# Análise do Git

Inspecione:

Branch Atual

Commit

Arquivos Modificados

Arquivos Deletados

Arquivos Adicionados

Arquivos Renomeados

Arquivos Staged

Arquivos Untracked

Histórico Recente

Nunca dependa exclusivamente do histórico do Git.

---

# Documentação Existente

Leia a documentação existente antes de gerar nova documentação.

Escopo de busca:

1. ~/obsidian/Projects/<Project>/

2. ~/obsidian/Knowledge/ quando o tema for conhecimento de engenharia reutilizável

Nunca leia ou escreva em outras pastas Projects/* na tarefa atual.

Priorize dentro do projeto atual:

README

INDEX

Architecture.md

ADR

Knowledge/Business

Knowledge/Troubleshooting

Knowledge/Infrastructure

Knowledge/Features

Knowledge/Bugs

Handoffs recentes

Releases

Nunca sobrescreva conhecimento estabelecido sem motivo.

---

# Sistema de Build

Determine como o projeto é construído.

Exemplos

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

Detecte frameworks de teste.

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

Identifique tecnologias de deploy.

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

# Níveis de Confiança

Toda detecção automática deve ter confiança.

High

Informação encontrada explicitamente.

Medium

Evidência forte.

Low

Inferência.

Unknown

Informação insuficiente.

Nunca converta premissas em fatos.

---

# Informação Ausente

Quando algo não puder ser detectado:

Registre.

Nunca invente.

Nunca alucine.

---

# Checklist de Qualidade da Detecção

Repositório identificado

Projeto identificado

Raiz do vault resolvida ou inicializada

Pasta do projeto resolvida ou inicializada a partir de project-template/

Stack identificada

Framework identificado

Infraestrutura identificada

Arquitetura inferida

Documentação do projeto consultada

Knowledge global consultado quando relevante

Outras pastas Projects não usadas como destinos de escrita

Confiança atribuída

Itens desconhecidos registrados

---

# Regra de Ouro

Entenda primeiro.

Documente depois.

Nunca inverta esta ordem.
