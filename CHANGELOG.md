# Changelog

Todas as mudanças relevantes deste projeto serão documentadas neste arquivo.

O formato segue Keep a Changelog.

O versionamento segue Semantic Versioning.

---

## [1.1.0]

### Adicionado

- Modos explícitos de leitura (início de tarefa) e escrita (fim de tarefa ou após PR/MR)
- Resolução do vault por `OBSIDIAN_VAULT`, path do WSL e `~/obsidian`
- Resolução do projeto pelo repositório remoto e pelo mapeamento do agent-kit (`ak-project`)

### Alterado

- Paths fixos `~/obsidian` substituídos por `$VAULT` em todas as regras

---

## [1.0.0]

### Adicionado

- Release inicial
- Memória de engenharia agnóstica de IA
- Integração com Obsidian
- Vault multi-projeto com isolamento
- Pasta global `Knowledge/`
- Bootstrap automático via `project-template/`
- Descoberta automática de projeto
- Captura de conhecimento
- Documentação de arquitetura
- Templates de handoff, ADR, feature, bug e demais tipos
- Instalação via `npx skills add igorsily/obsidian`
- Instruções e templates em Português Brasileiro
