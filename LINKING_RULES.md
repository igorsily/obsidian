# Engineering Memory
## Linking Rules

Version: 1.0.0

---

# Propósito

Conhecimento de engenharia nunca deve existir isolado.

Toda nota faz parte de um grafo de conhecimento maior.

A documentação se torna exponencialmente mais valiosa quando conceitos relacionados estão conectados.

O objetivo é criar uma base de conhecimento de engenharia navegável, e não uma coleção de documentos desconectados.

---

# Filosofia

Pense em relacionamentos.

Não pergunte:

"Qual nota estou escrevendo?"

Em vez disso, pergunte:

"Qual conhecimento já existe que se relaciona a isto?"

Toda nota deve ajudar engenheiros a descobrir outro conhecimento relevante.

---

# Wiki Links

Sempre prefira Wiki Links do Obsidian.

Prefira links path-qualified que permaneçam dentro do projeto atual ou apontem explicitamente para o Knowledge global.

Correto

[[Architecture]]

[[Knowledge/Infrastructure/Redis]]

[[Knowledge/Business/Owner Validation]]

[[ADR/ADR-003 Redis]]

[[Knowledge/Docker/Compose Patterns]]

Evite links nus quando houver ambiguidade.

Incorreto como padrão

[[Redis]]

[[Authentication]]

Evite links Markdown para documentação interna sempre que possível.

Wiki Links são o padrão.

---

# Isolamento de Projetos

Wiki links internos devem permanecer dentro do projeto atual.

Evite links que possam referenciar acidentalmente a documentação de outro projeto.

Busque e vincule apenas dentro de:

~/obsidian/Projects/<Project>/

e, quando relevante,

~/obsidian/Knowledge/

Nunca crie links que dependam de uma nota de outro Projects/* como destino primário.

---

# Links para Knowledge Global

Conhecimento de engenharia reutilizável fica na raiz do vault:

~/obsidian/Knowledge/<Area>/

Vincule com um path explícito sob o Knowledge global.

Exemplo

[[Knowledge/Spring/Transaction Boundaries]]

[[Knowledge/PostgreSQL/Indexing Patterns]]

[[Knowledge/Git/Rebase Workflow]]

Não confunda Knowledge global com:

Projects/<Project>/Knowledge/

Quando ambos os escopos puderem corresponder, use o path completo do vault que identifica a nota de forma única.

Exemplo

[[Projects/awesome-api/Knowledge/Infrastructure/Redis]]

[[Knowledge/Redis/Persistence]]

---

# Pensamento Bidirecional

Sempre que criar uma nota, pergunte:

Quais notas existentes devem apontar para cá?

Quais notas esta nota deve referenciar?

O conhecimento deve ser descoberta a partir de múltiplos pontos de entrada.

---

# Vincule Conhecimento Existente

Antes de salvar um documento:

Busque documentação relacionada nesta ordem:

1. Pasta do projeto atual

2. Pasta Knowledge global

Nunca busque outras pastas Projects/* por links relacionados para mesclar entre projetos.

Exemplos

Architecture

ADR

Knowledge/Business

Knowledge/Features

Knowledge/Infrastructure

Knowledge/Troubleshooting

Knowledge/Frameworks

Knowledge/Integrations

Handoffs recentes

Crie links sempre que existirem relacionamentos.

---

# Tipos de Link

Toda nota pode conter relacionamentos.

Exemplos

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

# Links de Handoff

Todo handoff deve referenciar:

Architecture

Business Rules

ADR

Features afetadas

Troubleshooting

Infrastructure

Notas de Framework

Handoffs relacionados

Exemplo

## Related Knowledge

[[Architecture]]

[[Knowledge/Business/Authentication Policy]]

[[ADR/ADR-003 Authentication]]

[[Knowledge/Infrastructure/JWT]]

[[Knowledge/Frameworks/Spring Security]]

---

# Links de Architecture

Notas de arquitetura devem referenciar

Business Rules

Infrastructure

Frameworks

ADR

Features

Database

API

Deployment

Nunca deixe a arquitetura isolada.

---

# Business Rules

Business Rules devem conectar a

Features

Architecture

Database

Validation

Troubleshooting

ADR

Nunca documente regras de negócio sem mostrar onde se aplicam.

---

# Links de ADR

Cada ADR deve referenciar

ADR anterior

Architecture afetada

Infrastructure relacionada

Business Rules

Handoff de implementação

ADR futuro

A arquitetura fica mais fácil de navegar quando as decisões estão conectadas.

---

# Notas de Framework

Notas de framework devem referenciar

Architecture

Features

Troubleshooting

Performance

Integrations

Evite documentação de framework isolada.

---

# Infrastructure

Infraestrutura deve referenciar

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

Troubleshooting deve referenciar

Framework afetado

Feature afetada

Architecture

Infrastructure

Business Rule

Bug conhecido

Nunca documente um problema sem vincular aos componentes afetados.

---

# Features

Features devem referenciar

Business Rules

Architecture

Infrastructure

ADR

Features relacionadas

Integrations

Troubleshooting

Handoffs recentes

---

# Bugs

Documentação de bugs deve referenciar

Feature

Architecture

Business Rule

Troubleshooting

Causa Raiz

ADR relacionado

Nunca documente bugs sem contexto.

---

# README

O README do projeto deve sempre vincular a

INDEX

Architecture

ADR

Knowledge/Business

Knowledge/Infrastructure

Knowledge/Frameworks

Knowledge/Integrations

Knowledge/Features

Knowledge/Troubleshooting

Handoffs mais recentes

O README é a homepage do projeto.

---

# INDEX

INDEX é o hub de navegação do projeto.

Deve vincular a

Handoffs recentes

Architecture

ADR

Knowledge/Business

Knowledge/Features

Knowledge/Infrastructure

Knowledge/Frameworks

Knowledge/Integrations

Knowledge/Troubleshooting

Knowledge/Bugs

Releases

README

O INDEX também pode vincular a notas relevantes do Knowledge global quando útil.

O INDEX nunca deve ficar desatualizado.

---

# Densidade de Links

Poucos links demais reduzem a descoberta.

Muitos links demais reduzem a legibilidade.

Prefira links significativos.

Evite vincular todo termo técnico.

---

# Links Duplicados

Não repita links idênticos várias vezes na mesma seção.

Uma referência significativa é suficiente.

---

# Confiança do Link

Só crie links quando existir um relacionamento significativo.

Nunca force conexões.

Qualidade é mais importante que quantidade.

---

# Links Quebrados

Se uma nota ainda não existir

Crie o wiki link mesmo assim.

Prefira um link path-qualified para que a nota futura caia no escopo correto.

Exemplo

[[Knowledge/Infrastructure/Caching]]

[[Architecture]]

Links quebrados nus são aceitáveis apenas quando o nome for único dentro do escopo de busca permitido.

Wiki links quebrados são aceitáveis.

---

# Nomenclatura de Links

Use nomes concisos com path suficiente para evitar colisões entre projetos.

Bom

[[Knowledge/Business/Payments]]

[[Knowledge/Infrastructure/Docker]]

[[Knowledge/Infrastructure/Redis]]

[[Architecture]]

Ruim

[[Complete Authentication Documentation]]

[[Docker Setup Documentation]]

[[Redis]]

quando múltiplos projetos podem ter uma nota Redis

---

# Seções de Navegação

Sempre que apropriado, termine notas com

---

## Related Notes

[[Architecture]]

[[Knowledge/Infrastructure/Redis]]

[[Knowledge/Frameworks/Spring Boot]]

[[ADR/ADR-002 Cache Strategy]]

[[Knowledge/Docker/Compose Patterns]]

---

## Related Handoffs

[[2026-07-09 Authentication Refactor]]

[[2026-08-14 JWT Improvements]]

---

## Related Business Rules

[[Knowledge/Business/Password Policy]]

[[Knowledge/Business/User Lifecycle]]

---

## Related Architecture

[[Architecture]]

[[Knowledge/Infrastructure/Caching]]

---

Esta seção melhora muito a descoberta.

---

# Grafo de Conhecimento

O objetivo não é apenas documentação.

O objetivo é construir um grafo de conhecimento de engenharia.

Há dois grafos conectados:

Grafo do projeto sob Projects/<Project>/

Grafo global sob Knowledge/

Toda tarefa concluída deve aumentar a conectividade do grafo relevante.

Nunca conecte projetos entre si por links nus acidentais.

O grafo deve ficar mais fácil de navegar com o tempo.

---

# Regra de Ouro

Nunca crie conhecimento isolado.

Todo conceito importante deve se conectar ao entendimento mais amplo do projeto ou ao conhecimento global de engenharia quando for reutilizável.
