# Engineering Memory

> Dê memória de engenharia de longo prazo aos seus agentes de IA com Obsidian.

Engineering Memory é um framework agnóstico de captura de conhecimento. Ele preserva conhecimento de engenharia de software entre conversas.

Em vez de gerar resumos descartáveis, o framework constrói continuamente uma base de conhecimento persistente.

---

## Filosofia

Toda tarefa de desenvolvimento gera conhecimento.

O conhecimento não deve desaparecer quando a conversa termina.

Documentação faz parte da implementação.

---

## Objetivos

- Preservar contexto de engenharia
- Capturar decisões arquiteturais
- Documentar regras de negócio
- Registrar histórico de implementação
- Isolar documentação por projeto
- Compartilhar conhecimento reutilizável de forma global
- Construir um segundo cérebro no Obsidian

---

## Instalação rápida

```bash
npx skills add igorsily/obsidian
```

Instalação global no Cursor:

```bash
npx skills add igorsily/obsidian -g -a cursor -y
```

Listar skills do repositório:

```bash
npx skills add igorsily/obsidian --list
```

Detalhes em [INSTALL.md](INSTALL.md).

---

## Funcionalidades

- Agnóstico de agente de IA
- Descoberta automática de projeto
- Inicialização automática de projeto
- Análise automática de repositório
- Vault Obsidian multi-projeto
- Pasta global `Knowledge/`
- Integração com Obsidian
- Wiki Links com path qualificado
- Geração de handoffs
- Geração de ADRs
- Extração de regras de negócio
- Documentação de troubleshooting
- Documentação de arquitetura
- Documentação incremental
- Deduplicação de conhecimento

---

## Agentes suportados

- Cursor
- Claude Code
- Codex
- Gemini CLI
- OpenAI Agents
- Qualquer assistente capaz de seguir instruções em Markdown

Instalação multi-agente via `npx skills`:

```bash
npx skills add igorsily/obsidian -a cursor -a claude-code -g
```

---

## Vault padrão

```
~/obsidian
```

---

## Estrutura de pastas

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

Novos projetos são inicializados a partir de `project-template/` neste repositório.

---

## Princípios

1. Nunca perder conhecimento.
2. Nunca duplicar documentação.
3. Explicar decisões.
4. Descobrir o contexto do projeto automaticamente.
5. Isolar a documentação por projeto.
6. Manter conhecimento de engenharia reutilizável no escopo global.
7. Conectar conhecimento com wiki links path-qualified.
8. Manter a documentação continuamente atualizada.
9. Escrever a documentação do vault em Português Brasileiro.

---

## Idioma

Instruções do skill, templates e documentação gerada no vault usam **Português Brasileiro**.

Nomes de pastas, paths e identificadores técnicos permanecem em inglês.

---

## Roadmap

Versão 1.0

- Fundação
- Vault multi-projeto
- Captura de conhecimento
- Templates
- Instalação via `npx skills`
- Documentação

Versões futuras podem estender integrações sem quebrar compatibilidade.

---

## Licença

MIT
