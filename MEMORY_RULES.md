# Engineering Memory
## Memory Rules

Version: 1.0.0

---

# Propósito

Nem toda informação merece armazenamento permanente.

O propósito destas regras é garantir que apenas conhecimento de engenharia valioso se torne parte da memória de longo prazo.

A base de conhecimento deve ficar mais útil com o tempo, não apenas maior.

Sempre otimize por sinal em vez de ruído.

---

# Roteamento de Armazenamento

Antes de salvar qualquer documento, determine:

Isto é conhecimento de engenharia reutilizável?

Se SIM

Armazene em

$VAULT/Knowledge/

Caso contrário

Armazene em

$VAULT/Projects/<Project>/

| Critério | Destino |
|---|---|
| Conhecimento de engenharia reutilizável entre projetos (Docker, Spring, Redis, Git, DDD, PostgreSQL, Linux, Java, Angular, AI) | $VAULT/Knowledge/<Area>/ |
| Conhecimento específico do projeto (business rules, features, bugs, ADRs, handoffs, releases, infraestrutura do projeto, troubleshooting do projeto, peculiaridades de framework do projeto) | $VAULT/Projects/<Project>/... |
| Rascunhos temporários e notas inacabadas | $VAULT/Inbox/ |

Nunca misture conhecimento de repositórios diferentes.

Nunca armazene notas específicas de projeto na pasta global Knowledge.

Nunca armazene notas globais de engenharia reutilizável dentro de uma pasta de projeto quando não forem específicas do projeto.

---

# Filosofia de Memória

Pense como um engenheiro de software experiente.

Pergunte a si mesmo:

"Se eu voltar a este projeto daqui a um ano, ficaria feliz que esta informação foi documentada?"

Se a resposta for não,

não armazene.

---

# Conhecimento de Longo Prazo

As informações a seguir devem ser preservadas quase sempre.

## Architecture

Exemplos

Limites do sistema

Módulos

Serviços

Fluxo de dados

Authentication

Caching

Messaging

Persistence

Infrastructure

API design

Relações de dependência

Modelo de deploy

---

## Business Rules

Documente conhecimento de negócio.

Exemplos

Quem pode executar uma ação.

Regras de validação.

Transições de estado.

Restrições de domínio.

Cálculos financeiros.

Regras de permissão.

Regras de ciclo de vida.

Nunca assuma que essas regras são óbvias.

---

## Decisões Técnicas

Documente toda decisão significativa.

Inclua:

Decisão

Motivo

Alternativas

Trade-offs

Consequências

Engenheiros futuros devem entender por que a decisão existe.

---

## Conhecimento de Infraestrutura

Preserve conhecimento sobre

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

Se o conhecimento for reutilizável entre projetos, armazene em:

$VAULT/Knowledge/

Se o conhecimento for específico do sistema atual, armazene em:

Projects/<Project>/Knowledge/Infrastructure/

---

## Conhecimento de Framework

Capture conhecimento de framework no escopo correto.

Peculiaridades de framework específicas do projeto pertencem a:

Projects/<Project>/Knowledge/Frameworks/

Exemplos

Spring Boot conventions used in this repository

Angular architecture choices in this codebase

Hibernate quirks discovered here

MapLibre configuration unique to this project

Conhecimento geral reutilizável de framework pertence a:

$VAULT/Knowledge/

Exemplos

Spring

Angular

React

Next.js

Evite copiar documentação oficial.

Preserve apenas conhecimento descoberto por trabalho real de engenharia.

---

## Troubleshooting

Preserve conhecimento operacional do projeto atual.

Documente:

Sintomas

Diagnóstico

Causa Raiz

Resolução

Prevenção

Armazene em:

Projects/<Project>/Knowledge/Troubleshooting/

Este conhecimento se torna extremamente valioso com o tempo.

---

## Performance

Documente descobertas de performance.

Exemplos

Queries caras.

Estratégias de cache.

Memory leaks.

Gargalos de thread.

Latência de rede.

Payloads grandes.

Decisões de otimização.

---

## Security

Documente decisões de segurança.

Authentication.

Authorization.

Encryption.

Secrets.

Rate limiting.

Audit logging.

Nunca exponha secrets.

---

## Integrations

Documente integrações externas.

Inclua

Propósito

Authentication

Limitações

Modos de falha

Dependências

---

# Conhecimento Temporário

Algumas informações não devem se tornar permanentes.

Exemplos

Discussão de hoje.

Ideias temporárias de implementação.

Brainstorming.

Rascunhos.

Trabalho em andamento.

Experimentos pela metade.

Notas de reunião.

Lembretes pessoais.

Mantenha informação temporária em:

$VAULT/Inbox/

Não trate notas do Inbox como memória permanente do projeto.

Promova conhecimento durável para a pasta correta do projeto ou Knowledge global.

---

# Não Armazene

Nunca preserve:

Saída aleatória de console

Logs de build

Erros temporários

Sessões de debug

Stack traces sem análise

Arquivos gerados

Opiniões pessoais

Transcrições de conversa

Informação repetida

Ruído

---

# Aprendizado

Sempre que algo inesperado for descoberto:

Pergunte:

"Outro engenheiro eventualmente encontrará isto?"

Se sim,

documente.

Caso contrário,

descarte.

---

# Detecção de Duplicatas

Antes de criar conhecimento:

Busque documentação existente nesta ordem:

1. $VAULT/Projects/<Project>/

2. $VAULT/Knowledge/

Nunca busque outras pastas Projects/* como destinos de escrita ou duplicatas para mesclar entre projetos.

Se um conceito equivalente já existir no escopo correto:

Atualize-o.

Não o duplique.

O conhecimento deve evoluir,

não se multiplicar.

---

# Ciclo de Vida do Conhecimento

Cada peça de conhecimento tem um de quatro estados.

## Active

Atual e preciso.

## Updated

Conhecimento existente melhorado.

## Deprecated

Ainda útil para contexto histórico.

## Archived

Não mais relevante.

Nunca delete conhecimento histórico de engenharia sem instrução explícita.

---

# Confiança

Ao documentar conhecimento inferido,

indique a confiança.

Exemplo

High

Medium

Low

Não apresente premissas como fatos.

---

# Completude

Documentação perfeita não é necessária.

Documentação útil é.

Se apenas parte do conhecimento estiver disponível,

documente o que for conhecido.

Identifique claramente as áreas desconhecidas.

---

# Checklist de Memória

Antes de salvar informação, pergunte:

Isto é conhecimento de engenharia reutilizável ou específico do projeto?

A pasta de destino está correta?

Isto será útil daqui a seis meses?

Explica uma decisão?

Explica uma regra de negócio?

Explica arquitetura?

Explica infraestrutura?

Previne erros futuros?

Ajuda outro engenheiro?

Se a maioria das respostas for "Não",

não armazene.

---

# Regra de Ouro

Armazene conhecimento.

Não conversas.

Armazene raciocínio.

Não histórico de chat.

Armazene entendimento.

Não informação bruta.

O propósito do Engineering Memory é preservar inteligência de engenharia,

não transcrições de conversa.
