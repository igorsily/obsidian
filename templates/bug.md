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

> Documentação de Defeito de Software

---

# Resumo

Forneça uma descrição concisa do defeito.

Foque no comportamento incorreto, não na implementação.

---

# Declaração do Problema

Descreva o defeito.

O que está acontecendo?

O que deveria acontecer?

Qual é a diferença?

---

# Comportamento Esperado

Descreva o comportamento esperado.

Use linguagem de negócio sempre que possível.

---

# Comportamento Atual

Descreva o comportamento observado.

Evite premissas.

Documente fatos.

---

# Impacto no Negócio

Descreva o impacto.

Exemplos

Cálculo incorreto

Perda financeira

Corrupção de dados

Interrupção de fluxo

Risco de segurança

Má experiência do usuário

Atrasos operacionais

---

# Severidade

Valores possíveis

Critical

High

Medium

Low

Informational

Explique por que esta severidade foi atribuída.

---

# Escopo

Descreva onde o bug ocorre.

Exemplos

Authentication

Payments

Registration

Reporting

Synchronization

Imports

API

UI

---

# Componentes Afetados

Liste os módulos afetados.

Exemplos

Authentication

OwnerService

Invoice API

Redis Cache

Angular UI

---

# Causa Raiz

Descreva a causa real.

Explique

Por que aconteceu

Por que não foi detectado antes

Problemas arquiteturais ou de negócio subjacentes

Evite explicações superficiais.

---

# Passos de Reprodução

Descreva como reproduzir.

Exemplo

1. Login

2. Abrir cadastro de Property

3. Adicionar segundo owner

4. Salvar

5. Observar ownership duplicado

A reprodução deve ser determinística sempre que possível.

---

# Pré-condições

Documente as condições necessárias.

Exemplos

Permissões específicas

Registros existentes

Configuração

Feature flags

Ambiente

---

# Resolução

Descreva a solução implementada.

Explique

O que mudou

Por que isso corrige o problema

Possíveis efeitos colaterais

---

# Validação

Descreva como a correção deve ser validada.

Inclua

Testes manuais

Testes automatizados

Testes de regressão

Casos extremos

Testes negativos

---

# Risco de Regressão

Descreva

Áreas que podem ser afetadas

Módulos relacionados

Dependências

Possíveis consequências indesejadas

---

# Prevenção

Explique como bugs semelhantes podem ser evitados.

Exemplos

Melhorias de arquitetura

Melhor validação

Testes adicionais

Análise estática

Monitoramento

Melhorias de code review

---

# Regras de Negócio Relacionadas

Referência

[[Knowledge/Business/Business Rule]]

---

# Features Relacionadas

Referência

[[Feature]]

---

# Arquitetura Relacionada

Referência

[[Architecture]]

---

# ADR Relacionado

Referência

[[ADR]]

---

# Troubleshooting Relacionado

Referência

[[Knowledge/Troubleshooting]]

---

# Handoffs Relacionados

Referencie o histórico de implementação.

---

# Lições Aprendidas

Descreva o conhecimento obtido.

Exemplos

Comportamento do framework

Mal-entendido de negócio

Fraqueza de arquitetura

Lacuna de validação

Premissa de infraestrutura

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
