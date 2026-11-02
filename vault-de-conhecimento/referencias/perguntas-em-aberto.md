# Perguntas em Aberto

> Etapa 7 do SKILL.md. Só introduza depois que o básico estiver funcionando. Com quem está começando, chame de "índice", nunca de "MOC".

**Como funciona:**
1. O consumo gerou uma pergunta sem resposta → crie uma nota para a **pergunta** (`tipo: pergunta`, `status: aberta`), dentro da área a que ela pertence, não junto do conteúdo de origem.
2. A nota da pergunta linka a origem: `· origem [[Nome do conteúdo]]`.
3. A pergunta entra no índice `Perguntas em Aberto`.
4. Quando aparecer dado, exemplo ou conversa que dialogue com ela, a pessoa abre a nota e adiciona, com a razão do link.
5. Quando amadurecer em decisão: `status: resolvida`, e a conclusão vai para a nota de destino (muitas vezes uma **Decisão**).

**Sem prazo.** É um radar, não uma lista de tarefas. Deixe isso explícito, ou a pessoa trata como pendência e abandona.

Um único conteúdo bem processado costuma abrir mais de uma pergunta, cada uma numa área diferente: uma sobre o trabalho, uma sobre o que a pessoa produz, uma sobre decisões futuras. Nenhuma delas é resumo; são linhas de pensamento próprio. É o argumento para quem acha que anotar é perda de tempo.

```markdown
---
tipo: indice
status: ativo
tags: [indice, perguntas]
criada: AAAA-MM-DD
---

# Perguntas em Aberto

> [!info] O que é isto
> Índice das provocações e perguntas em aberto que saem de aulas, livros, conteúdos e conversas, antes de virarem conclusão. Cada uma vive numa nota própria, na pasta do seu contexto. Sem prazo: é um radar, não uma lista de tarefas.

## Como usar
- Bateu num dado ou exemplo que dialoga com uma pergunta → abra a nota dela e linke, com a razão.
- A pergunta virou decisão → `aberta` → `resolvida`, e a conclusão vai para a nota de destino.

## Perguntas ativas
### [Área 1]
- [[Pergunta X]] — [a pergunta em uma linha] · origem [[Conteúdo Y]]

## Fontes que geraram perguntas
- [[Conteúdo Y]] — [o que era] (N perguntas)
```
