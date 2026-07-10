# Engineering Memory
## Project Rules

Version: 1.0.0

---

# Propósito

Estas regras definem como o conhecimento do projeto deve ser organizado.

O objetivo é criar uma base de conhecimento previsível, útil ao longo de meses ou anos de desenvolvimento.

Todo agente de IA deve seguir a mesma organização.

Consistência é mais importante do que preferência pessoal.

---

# Vault Padrão

O Vault Obsidian padrão é:

~/obsidian

Nunca pergunte ao usuário onde o Vault está localizado, a menos que a escrita falhe.

Se o Vault não existir:

- crie
- inicialize a estrutura de diretórios do vault
- continue normalmente

Estrutura da raiz do vault:

```
~/obsidian/

    Projects/

    Knowledge/

    Templates/

    Inbox/
```

Nunca peça ao usuário para escolher onde a documentação é armazenada.

---

# Descoberta de Projeto

Cada repositório deve mapear para exatamente uma pasta de projeto.

Exemplo

Repositório

awesome-api

torna-se

~/obsidian/Projects/awesome-api/

Nunca crie múltiplas pastas de projeto para o mesmo repositório.

Se a pasta do projeto não existir:

- copie a estrutura de `project-template/` neste repositório da skill
- coloque em `~/obsidian/Projects/<Project>/`
- continue normalmente

Nunca peça confirmação antes de inicializar um projeto.

---

# Estrutura de Diretórios do Vault

O Vault Obsidian deve seguir esta estrutura.

```
~/obsidian/

    Projects/

        <Project>/

            INDEX.md

            README.md

            Architecture.md

            ADR/

            Handoffs/

            Releases/

            Knowledge/

                Business/

                Features/

                Bugs/

                Infrastructure/

                Integrations/

                Troubleshooting/

                Frameworks/

    Knowledge/

        Java/

        Spring/

        Angular/

        Docker/

        PostgreSQL/

        Redis/

        Linux/

        Git/

        AI/

    Templates/

    Inbox/
```

Nunca renomeie estas pastas.

Nunca localize nomes de pastas.

Sempre use inglês nos nomes de pastas.

---

# Isolamento de Projetos

Cada projeto possui sua própria documentação.

Conhecimento de repositórios diferentes nunca deve ser misturado.

Nunca escreva notas específicas de um projeto na pasta de outro projeto.

Nunca armazene conhecimento específico de projeto na pasta global `Knowledge/`.

---

# Knowledge Global

Conhecimento de engenharia reutilizável pertence a:

~/obsidian/Knowledge/

Exemplos

Docker

Spring

Redis

Linux

DDD

PostgreSQL

Git

Java

Angular

AI

O conhecimento global é compartilhado entre todos os projetos.

---

# Knowledge do Projeto

Conhecimento específico do projeto sempre pertence a:

~/obsidian/Projects/<Project>/

Exemplos

Business Rules

Architecture

Features

Infrastructure

Integrations

Troubleshooting

Bugs

ADRs

Releases

Handoffs

Peculiaridades de framework descobertas no repositório

---

# Bootstrap de Projeto

Quando um novo projeto é detectado e `~/obsidian/Projects/<Project>/` não existe:

1. Garanta que a raiz do vault exista com `Projects/`, `Knowledge/`, `Templates/` e `Inbox/`
2. Replique `project-template/` em `~/obsidian/Projects/<Project>/`
3. Continue a documentação normalmente

A fonte da verdade do bootstrap é:

project-template/

dentro do repositório da skill Engineering Memory.

---

# README

Todo projeto deve conter um README.

O README representa o estado atual do projeto.

Deve ser atualizado ao longo do tempo.

Nunca deve se tornar um log histórico.

Em vez disso, deve responder:

O que é este projeto?

Quais tecnologias são usadas?

Como está organizado?

Como pode ser executado?

Quais sistemas externos existem?

O que um novo engenheiro deve saber?

---

# INDEX

Todo projeto contém um INDEX.

O INDEX é o ponto de entrada de navegação.

Ele vincula:

Handoffs recentes

Architecture

ADR

Knowledge/Business

Knowledge/Features

Knowledge/Infrastructure

Knowledge/Integrations

Knowledge/Troubleshooting

Knowledge/Frameworks

Knowledge/Bugs

Releases

O INDEX deve sempre refletir a documentação atual.

---

# Handoffs

Handoffs descrevem trabalho concluído.

Cada handoff representa uma implementação lógica.

Use nomes de arquivo como

YYYY-MM-DD HH-mm - Task Name.md

Nunca sobrescreva um handoff.

Handoffs são registros históricos imutáveis.

Armazene em:

Projects/<Project>/Handoffs/

---

# Architecture

Notas de arquitetura descrevem conceitos técnicos de longo prazo.

A visão geral da arquitetura do projeto fica em:

Projects/<Project>/Architecture.md

Notas adicionais de arquitetura podem ficar ao lado ou ser vinculadas a partir dela.

Exemplos

Authentication

Caching

Messaging

Database

API

Microservices

Domain Model

Notas de arquitetura evoluem ao longo do tempo.

Atualize-as.

Não crie duplicatas.

---

# ADR

Architecture Decision Records documentam decisões técnicas importantes.

Crie um ADR sempre que uma decisão alterar:

Architecture

Infrastructure

Database

Framework

Deployment

Messaging

Authentication

Caching

Storage

Um ADR por decisão.

Armazene em:

Projects/<Project>/ADR/

---

# Business Rules

Business Rules descrevem conhecimento de domínio.

Exemplos

Owner can have only one active property.

Invoices cannot be cancelled after payment.

Users cannot delete themselves.

Business Rules devem evitar detalhes de implementação.

Descreva o domínio.

Armazene em:

Projects/<Project>/Knowledge/Business/

---

# Features

Cada feature concluída pode receber sua própria documentação.

Descreva:

Propósito

Comportamento

Dependências

Limitações

Melhorias futuras

Armazene em:

Projects/<Project>/Knowledge/Features/

---

# Bugs

Documente bugs recorrentes.

Inclua

Sintomas

Causa

Solução

Workaround

Status

Nunca documente falhas temporárias.

Apenas conhecimento recorrente.

Armazene em:

Projects/<Project>/Knowledge/Bugs/

---

# Infrastructure

Notas de infraestrutura descrevem infraestrutura específica do projeto.

Exemplos

Docker setup for this project

Kubernetes manifests used here

Redis usage in this system

Deployment topology

Secrets layout

Armazene em:

Projects/<Project>/Knowledge/Infrastructure/

Conhecimento de infraestrutura reutilizável entre projetos pertence a:

~/obsidian/Knowledge/

---

# Frameworks

Notas de framework sob o projeto documentam apenas conhecimento específico do projeto.

Exemplos

Spring Boot conventions used in this repository

Angular architecture choices in this codebase

Hibernate quirks discovered here

Armazene em:

Projects/<Project>/Knowledge/Frameworks/

Conhecimento geral de framework pertence a:

~/obsidian/Knowledge/

Evite copiar documentação oficial.

---

# Integrations

Documente sistemas externos usados pelo projeto.

Exemplos

Stripe

Google Maps

Cloudflare

AWS

Azure

SMTP

OAuth

REST APIs

Armazene em:

Projects/<Project>/Knowledge/Integrations/

---

# Troubleshooting

Documente problemas operacionais recorrentes deste projeto.

Inclua

Problema

Diagnóstico

Causa Raiz

Resolução

Prevenção

Armazene em:

Projects/<Project>/Knowledge/Troubleshooting/

---

# Releases

Notas de release pertencem a:

Projects/<Project>/Releases/

---

# Inbox

Rascunhos temporários e notas inacabadas pertencem a:

~/obsidian/Inbox/

Nunca trate o conteúdo do Inbox como memória permanente do projeto.

Promova conhecimento durável para a pasta correta do projeto ou global.

---

# Templates

Templates do vault ficam em:

~/obsidian/Templates/

Templates da skill ficam em:

templates/

dentro do repositório da skill Engineering Memory.

Prefira templates da skill ao gerar documentação.

---

# Nomenclatura

Prefira nomes concisos.

Bom

Authentication

Caching

Payments

Owners

Ruim

Authentication Documentation Final Version

---

# Datas

Sempre use datas ISO.

Exemplo

2026-07-09

Nunca use formatos específicos de locale.

---

# Links

Sempre crie wiki links.

Prefira links path-qualified para preservar o isolamento de projetos.

Exemplo

[[Architecture]]

[[Knowledge/Business/Owner Validation]]

[[Knowledge/Infrastructure/Redis]]

[[ADR/ADR-001 Authentication]]

Para conhecimento global de engenharia:

[[Knowledge/Docker/Compose Patterns]]

Siga LINKING_RULES.md para as regras de isolamento.

O conhecimento deve se tornar um grafo conectado.

---

# Propriedade

Conhecimento específico do projeto pertence ao projeto.

Conhecimento de engenharia reutilizável pertence à pasta global Knowledge.

Nunca referencie conversas individuais.

Nunca referencie contexto temporário de chat.

A documentação deve sobreviver ao desaparecimento de qualquer sessão de IA.

---

# Atualização

Quando a informação mudar:

Atualize a nota existente.

Não crie outra nota.

A evolução histórica pertence ao Git.

Não a notas duplicadas.

---

# Princípio

Um projeto deve ficar mais fácil de entender após cada tarefa concluída.

Nunca deixe a documentação pior do que estava antes.
