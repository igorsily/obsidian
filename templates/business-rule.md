---
type: business-rule

id:

status: Active

project:

domain:

owners:
  - AI

created:

updated:

tags:
  - business
---

# {{title}}

> Regra de Negócio

---

# Propósito

Descreva a regra de negócio.

O que esta regra garante?

Quem é afetado?

Por que esta regra existe?

---

# Contexto de Negócio

Explique o processo de negócio.

Onde esta regra se aplica?

Quais usuários estão envolvidos?

Qual evento de negócio a dispara?

---

# Descrição da Regra

Descreva a regra em linguagem simples.

Evite detalhes de implementação.

Bom exemplo

Apenas um owner ativo pode existir para uma property.

Mau exemplo

Validate owner.active == true.

---

# Motivação

Explique por que esta regra existe.

Exemplos

Requisito legal

Regra financeira

Processo operacional

Requisito de segurança

Requisito do cliente

Restrição legada

---

# Escopo

Descreva onde a regra se aplica.

Exemplos

Registration

Authentication

Payments

Invoices

Properties

Users

Notifications

Imports

Exports

---

# Pré-condições

O que deve ser verdadeiro antes desta regra se aplicar?

Exemplo

A property já existe.

O usuário está autenticado.

A invoice está em aberto.

---

# Regra

Descreva a regra com precisão.

Se útil, divida em passos.

Exemplo

1. Validar ownership.

2. Verificar contratos ativos.

3. Rejeitar duplicatas.

4. Persistir ownership.

---

# Exceções

Liste situações em que a regra não se aplica.

Explique o motivo.

---

# Validação

Como a regra deve ser validada?

Exemplos

Validação de UI

Validação de API

Constraint de banco de dados

Processo agendado

Background worker

---

# Comportamento em Erro

Descreva o que acontece quando a regra é violada.

Exemplo

HTTP 409

Mensagem de validação

Rollback

Log de auditoria

Notificação

---

# Impacto no Negócio

Descreva o que acontece se esta regra for removida ou ignorada.

Exemplos

Invoices duplicadas

Ownership inválido

Inconsistência financeira

Corrupção de dados

Problemas legais

---

# Dependências

Referencie regras relacionadas.

Exemplos

[[Property Lifecycle]]

[[Owner Validation]]

[[Authentication]]

---

# Features Relacionadas

Referencie features afetadas.

Exemplos

[[Property Registration]]

[[Transfer Ownership]]

---

# Arquitetura Relacionada

Exemplos

[[Properties]]

[[Authentication]]

[[Database]]

---

# ADR Relacionado

Referencie decisões de arquitetura.

Exemplos

[[ADR-004 Ownership Model]]

---

# Handoffs Relacionados

Referencie o histórico de implementação.

Exemplos

[[2026-07-12 Property Ownership]]

---

# Exemplos

Forneça exemplos práticos.

## Válido

Property A

Owner John

Status Active

Aceito

---

## Inválido

Property A

Owner John

Owner Mary

Ambos Active

Rejeitado

---

# Casos Extremos

Descreva situações incomuns.

Exemplos

Migração

Imports

Dados legados

Usuários excluídos

Properties arquivadas

---

# Considerações Futuras

Descreva possíveis mudanças futuras.

Exemplos

Ownership múltiplo

Ownership temporário

Co-ownership

Legislação internacional

---

# Metadata

Business Area

Repository

Branch

Commit

Confidence

Last Review

Generated At
