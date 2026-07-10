# Instalação

## Requisitos

- Qualquer agente de IA capaz de seguir instruções em Markdown
- Obsidian (recomendado)
- Git
- Node.js (para `npx skills`)

---

## Instalação recomendada (`npx skills`)

```bash
npx skills add igorsily/obsidian
```

### Global no Cursor

```bash
npx skills add igorsily/obsidian -g -a cursor -y
```

### Listar skills do repositório

```bash
npx skills add igorsily/obsidian --list
```

### Vários agentes

```bash
npx skills add igorsily/obsidian -a cursor -a claude-code -g
```

O CLI instala o skill em pastas como:

- Cursor global: `~/.cursor/skills/`
- Cursor/projeto: `.agents/skills/` ou equivalente do agente

---

## Clone manual

```bash
git clone https://github.com/igorsily/obsidian.git
```

Depois copie a pasta do skill para o diretório de skills do seu agente, por exemplo:

```bash
cp -r obsidian ~/.cursor/skills/engineering-memory
```

---

## Vault

O vault padrão fica em:

```
~/obsidian
```

Se não existir, o skill deve criá-lo automaticamente com:

```
Projects/
Knowledge/
Templates/
Inbox/
```

Cada repositório detectado mapeia para:

```
~/obsidian/Projects/<Project>/
```

Se a pasta do projeto não existir, o skill inicializa a partir de `project-template/` sem pedir confirmação.

Conhecimento de engenharia reutilizável fica em:

```
~/obsidian/Knowledge/
```

---

## Verificação

Após instalar, o agente deve:

- detectar repositórios
- resolver ou criar a pasta do projeto correspondente
- descobrir frameworks
- gerar handoffs
- gravar docs do projeto em `Projects/<Project>/`
- gravar conhecimento reutilizável em `Knowledge/`
- atualizar documentação
- criar notas de arquitetura
- manter memória isolada por projeto
- escrever a documentação do vault em Português Brasileiro

---

## Atualização

```bash
npx skills update engineering-memory
```

Ou reinstale:

```bash
npx skills add igorsily/obsidian -g -a cursor -y
```
