---
name: engineering-memory
version: 1.0.0
author: Igor Sily
description: Framework de memória de engenharia para Obsidian. Use ao documentar handoffs, ADRs, arquitetura, regras de negócio, troubleshooting ou ao preservar conhecimento de projetos de software.
---

# Engineering Memory

## Missão

Sua responsabilidade não é apenas implementar software.

Sua responsabilidade é preservar conhecimento de engenharia.

Toda tarefa concluída deve deixar o projeto mais fácil de entender do que antes.

Assuma que toda conversa eventualmente desaparecerá.

A documentação se torna a memória de longo prazo do projeto.

A implementação só está completa quando o conhecimento relevante foi preservado.

---

# Idioma da Documentação

Toda documentação gerada no vault deve ser escrita em Português Brasileiro (PT-BR).

Exceções obrigatórias — mantenha em inglês:

- nomes de pastas do vault (`Projects/`, `Knowledge/`, `ADR/`, `Handoffs/`, `Releases/`, `Inbox/`, `Templates/`, etc.)
- paths e wiki links path-qualified
- identificadores técnicos (nomes de frameworks, ferramentas, arquivos de configuração, commits, branches)

Nunca localize nomes de pastas do vault.

---

# Objetivos Primários

Sempre busque:

- Preservar contexto
- Preservar raciocínio
- Preservar decisões
- Preservar descobertas
- Preservar conhecimento de negócio
- Preservar conhecimento arquitetural
- Preservar conhecimento de troubleshooting

Nunca reduza a documentação a um resumo simples.

---

# Base de Conhecimento Padrão

Salvo instrução explícita em contrário, a base de conhecimento fica em:

~/obsidian

Estrutura esperada do vault:

```
~/obsidian/

    Projects/

    Knowledge/

    Templates/

    Inbox/
```

Se não existir:

- crie
- inicialize a estrutura de diretórios esperada
- continue normalmente

Nunca pergunte ao usuário onde salvar documentação, a menos que a escrita no local padrão falhe.

---

# Isolamento de Projetos

Cada projeto possui sua própria documentação.

Conhecimento de repositórios diferentes nunca deve ser misturado.

Conhecimento específico de projeto sempre pertence a:

~/obsidian/Projects/<Project>/

Conhecimento de engenharia reutilizável pertence a:

~/obsidian/Knowledge/

Nunca escreva na pasta de outro projeto.

---

# Detecção Automática de Projeto

Antes de documentar qualquer coisa, detecte o repositório atual e determine o nome do projeto.

Mapeie o repositório para:

~/obsidian/Projects/<Project>/

O usuário nunca deve precisar escolher manualmente onde a documentação é armazenada.

Siga DETECTION_RULES.md e PROJECT_RULES.md.

---

# Criação Automática de Projeto

Se a pasta do projeto detectado não existir:

- inicialize replicando `project-template/`
- continue normalmente

Nenhuma confirmação é necessária.

---

# Descoberta do Repositório

Antes de documentar qualquer coisa, inspecione o repositório.

Determine, quando possível:

- Nome do Projeto
- Nome do Repositório
- URL do Repositório
- Branch Atual
- Commit Atual
- Monorepo ou Repositório Único
- Estrutura do Workspace
- Tecnologias Backend
- Tecnologias Frontend
- Stack de Infraestrutura
- Ferramentas de Build
- Gerenciadores de Pacotes
- Linguagens de Programação
- Frameworks de Teste
- Estratégia de Deploy
- Plataforma de CI/CD
- Estilo de Arquitetura

Use todas as fontes disponíveis, incluindo:

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
- estrutura do repositório

Nunca invente informação.

Se estiver incerto, registre explicitamente que a informação não pôde ser determinada.

---

# Entenda o Trabalho Atual

Antes de escrever documentação, entenda o que foi realmente realizado.

Use todas as fontes disponíveis:

- arquivos modificados
- git diff
- arquivos staged
- mensagem de commit
- contexto do repositório
- conversa atual

Infira:

- objetivo
- módulos afetados
- impacto arquitetural
- impacto de negócio
- impacto de infraestrutura

---

# Leia o Conhecimento Existente Primeiro

Antes de criar qualquer documentação nova:

1. Resolva ~/obsidian/Projects/<Project>/
2. Leia o conhecimento existente dentro dessa pasta do projeto
3. Quando o tema for conhecimento de engenharia reutilizável, consulte também ~/obsidian/Knowledge/
4. Nunca use outra pasta Projects/* como fonte ou destino de escrita da tarefa atual

Priorize:

Project README

INDEX

Architecture.md

Knowledge/Business

ADR

Knowledge/Troubleshooting

Handoffs recentes

Knowledge/Features

Knowledge/Bugs

Releases

Knowledge/Infrastructure

Knowledge/Frameworks

Knowledge/Integrations

A base de conhecimento existente é a fonte primária da verdade.

Evite contradizer documentação anterior.

---

# Captura de Conhecimento

Ao final de toda tarefa concluída:

Capture:

## O que foi construído

## Por que foi construído

## Como funciona

## Premissas importantes

## Trade-offs

## Lições aprendidas

## Conhecimento de negócio descoberto

## Conhecimento arquitetural descoberto

## Conhecimento de infraestrutura descoberto

## Limitações de framework descobertas

## Riscos

## Melhorias futuras

---

# Geração de Handoff

Gere um handoff descrevendo o trabalho concluído.

O handoff deve permitir que outro engenheiro continue o projeto sem acesso às conversas anteriores.

O handoff deve explicar:

Contexto

Objetivo

Implementação

Decisões Técnicas

Impacto na Arquitetura

Arquivos Alterados

Validação

Trabalho Pendente

Lições Aprendidas

Metadados

---

# Extração de Conhecimento

Nem tudo pertence a um handoff.

Detecte conhecimento reutilizável.

Exemplos:

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

Antes de armazenar, decida o destino:

Conhecimento de engenharia reutilizável entre projetos

→ ~/obsidian/Knowledge/

Conhecimento específico do projeto

→ ~/obsidian/Projects/<Project>/

Armazene conhecimento reutilizável separado de handoffs e de notas exclusivas do projeto.

---

# Regras de Documentação

Sempre prefira:

Atualizar notas existentes

em vez de

Criar notas duplicadas.

Nunca crie múltiplas notas descrevendo o mesmo conceito.

---

# Wiki Links

Sempre que possível, crie wiki links do Obsidian.

Prefira links path-qualified para preservar o isolamento de projetos.

Exemplo:

[[Architecture]]

[[Knowledge/Business/Owner Validation]]

[[Knowledge/Infrastructure/Redis]]

[[ADR/ADR-003 Redis]]

Para conhecimento global de engenharia:

[[Knowledge/Docker/Compose Patterns]]

[[Knowledge/Spring/Transaction Boundaries]]

Evite links nus como [[Redis]] ou [[Authentication]] quando o nome puder existir em outro projeto.

Vincule notas relacionadas sempre que existir uma relação.

Siga LINKING_RULES.md.

---

# Estilo de Escrita

Escreva para engenheiros.

Assuma que o leitor entra no projeto daqui a seis meses.

Explique o raciocínio.

Explique trade-offs.

Explique decisões.

Explique consequências.

Evite resumos genéricos.

Capture conhecimento oculto.

---

# Checklist de Qualidade

Antes de considerar a documentação completa, verifique:

✓ Repositório identificado

✓ Pasta do projeto resolvida ou inicializada

✓ Tecnologias identificadas

✓ Conhecimento existente do projeto consultado

✓ Knowledge global consultado quando relevante

✓ Documentação armazenada no escopo correto

✓ Notas duplicadas evitadas

✓ Wiki links path-qualified criados

✓ Decisões técnicas documentadas

✓ Regras de negócio documentadas

✓ Riscos documentados

✓ Validação documentada

✓ Trabalho futuro documentado

---

# Critérios de Conclusão

Uma tarefa só é considerada completa quando:

- a implementação está finalizada
- a documentação está atualizada
- o conhecimento reutilizável foi extraído
- a memória do projeto foi preservada

Documentação faz parte da implementação.

Nunca considere apenas o código como tarefa concluída.
