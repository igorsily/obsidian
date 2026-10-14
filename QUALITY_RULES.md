# Engineering Memory
## Quality Rules

Version: 1.0.0

---

# Propósito

Documentação faz parte da implementação.

Documentação ruim cria dívida técnica futura.

Antes de armazenar qualquer conhecimento, avalie sua qualidade.

O objetivo não é maximizar a quantidade de documentação.

O objetivo é maximizar a utilidade.

---

# Filosofia de Documentação

Boa documentação responde perguntas.

Ótima documentação previne perguntas.

Sempre otimize para entendimento futuro.

Imagine um engenheiro lendo esta documentação daqui a um ano.

Ele entenderá por que a decisão foi tomada?

Se não,

melhore a documentação.

---

# Definition of Done

Uma tarefa de desenvolvimento só está completa quando:

✓ O código está implementado.

✓ Os testes foram executados quando aplicável.

✓ A documentação foi atualizada.

✓ O conhecimento foi extraído.

✓ Notas existentes foram atualizadas.

✓ Documentação duplicada foi evitada.

Só então a tarefa está completa.

---

# Perguntas de Engenharia

Todo documento deve responder o máximo possível destas perguntas.

O que mudou?

Por que foi necessário?

Como funciona?

Quais premissas existem?

Quais trade-offs foram feitos?

Quais alternativas foram rejeitadas?

Quais riscos permanecem?

Como pode ser testado?

O que outro engenheiro deve saber?

---

# Explique o Porquê

Nunca pare em descrever o que aconteceu.

Sempre explique o porquê.

Ruim

"Redis was added."

Bom

"Redis was introduced to reduce repeated database access for frequently requested reference data. Local in-memory caching was rejected because multiple application instances require shared cache consistency."

O raciocínio é mais valioso do que detalhes de implementação.

---

# Decisões Técnicas

Toda decisão significativa deve incluir

Decisão

Motivação

Alternativas

Trade-offs

Consequências

Implicações futuras

Se isto não puder ser explicado,

a decisão não foi documentada corretamente.

---

# Evite Documentação de Baixo Valor

Não escreva documentação que apenas repete o código.

Ruim

"The UserService contains methods."

Bom

"The UserService centralizes permission validation to avoid duplicated authorization logic across controllers."

A documentação deve explicar a intenção.

O código já explica a sintaxe.

---

# Explique Premissas

Sempre que existirem premissas,

documente-as.

Exemplos

Restrições esperadas do banco de dados

Comportamento esperado da API

Topologia de deploy esperada

Limitações de framework

Premissas de performance

Premissas de segurança

Premissas ocultas criam bugs futuros.

---

# Informação Desconhecida

É aceitável documentar incerteza.

Exemplo

"The deployment strategy could not be determined automatically."

Nunca invente informação ausente.

---

# Preservação de Contexto

Engenheiros futuros não devem precisar de acesso a:

Histórico de chat

Pull Requests

Reuniões

Slack

Email

Tudo o que for necessário já deve existir na base de conhecimento do projeto atual, com links para o Knowledge global quando o contexto de engenharia for reutilizável.

---

# Concisão

A documentação deve ser concisa.

Remova repetição.

Remova preenchimento.

Remova afirmações óbvias.

Mantenha as explicações completas.

Evite verbosidade desnecessária.

---

# Precisão Técnica

Precisão é mais importante que completude.

Documentação incompleta mas correta é melhor do que documentação completa mas incorreta.

Nunca especule.

---

# Reuso de Conhecimento

Antes de escrever:

Busque documentação existente nesta ordem:

1. $VAULT/Projects/<Project>/

2. $VAULT/Knowledge/

Nunca busque outras pastas Projects/* por conteúdo para mesclar.

Se conhecimento equivalente existir no escopo correto:

Atualize-o.

Não o duplique.

O conhecimento deve evoluir.

Não se multiplicar.

---

# Exemplos

Sempre que um conceito for difícil,

inclua um exemplo.

Exemplos melhoram drasticamente a compreensão.

Prefira exemplos práticos a explicações teóricas.

---

# Audiência

Escreva para

Engenheiros

Arquitetos

Agentes de IA futuros

Assuma leitores técnicos.

Não simplifique demais.

---

# Linguagem

Seja objetivo.

Evite linguagem de marketing.

Evite opiniões.

Evite adjetivos desnecessários.

Prefira linguagem técnica precisa.

A documentação gerada no vault deve ser escrita em Português Brasileiro (PT-BR), exceto nomes de pastas, paths e identificadores técnicos.

---

# Confiança

Toda afirmação inferida deve incluir confiança.

High

Medium

Low

Unknown

Nunca apresente premissas como fatos.

---

# Score de Documentação

Antes de salvar a documentação,

avalie as seguintes categorias.

Architecture

★★★★★

Business Rules

★★★★★

Implementation

★★★★★

Technical Decisions

★★★★★

Validation

★★★★★

Troubleshooting

★★★★★

Infrastructure

★★★★★

Knowledge Reuse

★★★★★

Links

★★★★★

Completeness

★★★★★

Categorias com baixa qualidade devem ser melhoradas antes de salvar.

---

# Auto Revisão

Antes de finalizar,

revise a documentação.

Pergunte a si mesmo

Outro engenheiro entenderia isto?

Outra IA continuaria o trabalho?

Eu entenderia isto daqui a um ano?

Se a resposta for "Não",

continue melhorando.

---

# Checklist de Conclusão

Repositório entendido

Pasta do projeto resolvida ou inicializada

Tarefa entendida

Impacto na arquitetura documentado

Impacto de negócio documentado

Decisões técnicas documentadas

Riscos documentados

Validação documentada

Conhecimento extraído

Documento armazenado no escopo correto

Sem escritas em outras pastas Projects/*

Notas existentes atualizadas

Notas duplicadas evitadas

Wiki links path-qualified criados quando houver ambiguidade

Metadados incluídos

Confiança registrada

Qualidade revisada

---

# Regra de Ouro

O objetivo não é documentar tudo.

O objetivo é preservar entendimento.

O entendimento sobrevive à implementação.

O código muda.

O conhecimento permanece.
