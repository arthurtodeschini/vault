# Moldes de nota

> Comece com no máximo 2 (Etapa 3 do SKILL.md). Salve em `Templates/` e adapte ao vocabulário da pessoa; não copie cru. Os valores de `tipo` e `status` seguem `vocabulario.md`.

| Template | Use quando o gatilho for... |
|---|---|
| Conteúdo | palestra, post, podcast, vídeo, curso, artigo |
| Evento | evento, imersão ou curso com várias palestras |
| Decisão | decisão relevante e repetível |
| Nota viva + Fotografia | algo com um estado atual que muda |
| Aula | aula de faculdade ou curso com sequência |
| Projeto | projeto com começo, meta e fim |
| Livro | leitura |
| Captura rápida | coisas que chegam sem forma |

---

## Template — Conteúdo (palestra, post, podcast, curso)

```markdown
---
tipo: conteudo
formato: 
autor: 
fonte: 
evento: 
data: 
status: rascunho
tags: []
---

# [Título] ([Autor])

> [!note] Fontes
> De onde veio cada parte desta nota (caderno, fotos dos slides, post, vídeo).

## A tese central
> O argumento principal em um parágrafo. Se não couber, ainda não foi entendido.

## O conteúdo
> Os modelos e argumentos, com o diagrama embutido onde o conceito aparece.

## Key insights
> No máximo 3. O que muda a forma de pensar.

## Insight prático
> Pelo menos 1. O que eu faço diferente a partir de segunda-feira.

## Como se aplica ao meu caso
> [!question] Leitura do Claude — pra validar
> (reescrever com as minhas palavras)

## Provocação que ficou
> Pergunta sem resposta? Criar nota própria e indexar em [[Perguntas em Aberto]].

## Conexões
- [[ ]] — por quê
```

## Template — Evento (hub)

Um evento com várias palestras ganha **uma pasta própria** (com subpasta por dia, se durar mais de um dia). Dentro dela: esta nota-hub + uma nota de **Conteúdo** por palestra.

```markdown
---
tipo: evento
data: 
local: 
status: em-andamento
tags: [evento]
---

# [Nome do evento]

## Meus 3 objetivos com este evento
> Escritos ANTES de começar. O que eu quero sair sabendo ou resolvendo?
1. 
2. 
3. 

## Método de anotação
Por palestra: a tese em uma frase, até 3 key insights e **pelo menos 1 insight prático**.

## Palestras
## Dia 1 — DD/MM
- [[Palestrante - Título]] — a ideia central em uma linha

## O que levo
> Escrito por mim, depois do evento. Responde aos 3 objetivos.

| Objetivo | O que encontrei (e em qual palestra) | Próxima ação |
|---|---|---|

## Conexões
- [[ ]] — por quê
```

**Por que esse formato funciona:** os 3 objetivos transformam "assistir" em "procurar", e o "O que levo" obriga o fechamento. A lista com uma linha por palestra vira o índice que a pessoa realmente relê.

## Template — Decisão

Para decisões relevantes e repetíveis. A nota mais valiosa do vault no longo prazo: daqui a um ano, a pessoa consegue ver **o que pensava na hora**, e não só o que aconteceu.

```markdown
---
tipo: decisao
status: tomada
data: 
area: 
revisar-em: 
tags: [decisao]
---

# Decisão — AAAA-MM-DD — [assunto]

> [!summary] Em uma linha
> O que eu decidi e o critério principal.

## 1. Contexto
> O que estava acontecendo, com números.

## 2. O que eu pensava antes
> As hipóteses e expectativas na hora. Não editar depois.

## 3. Decisão
| # | Decisão | Execução | Por quê |
|---|---|---|---|

## 4. Alternativas descartadas
- [alternativa] — por que não

## 5. Riscos que aceitei conscientemente

## 6. O que me faria mudar de ideia
> E quando revisar (campo `revisar-em`).

## 7. Aprendizados
> Preencher na revisão. Aí o status vira `revisada`.

## Conexões
- [[ ]] — por quê
```

## Template — Nota viva + Fotografia

Para qualquer coisa que tenha um **estado atual** que muda: carteira de investimentos, orçamento, metas, funil de clientes, status de um projeto grande.

O erro clássico é um de dois: sobrescrever e perder o histórico, ou criar doze versões sem saber qual é a atual. A solução são duas notas com papéis diferentes:

- **Nota viva** (`[Nome] atual`): uma só, sempre sobrescrita. É a fonte única do estado de hoje.
- **Fotografia** (`[Nome] — AAAA-MM-DD`): cópia congelada, criada quando algo relevante acontece (uma decisão, o fechamento do mês). Nunca muda.

```markdown
---
tipo: nota-viva
status: ativa
atualizada: AAAA-MM-DD
tags: []
---

# [Nome] atual

> [!info] Como usar esta nota
> Fonte única do estado atual. É sobrescrita a cada atualização.
> O histórico fica nas fotografias datadas (ver Log).

## Resumo
## [Seções do estado atual]

## Log de atualizações
| Data | O que mudou | Fotografia |
|---|---|---|
| AAAA-MM-DD | | [[Nome — AAAA-MM-DD]] |
```

```markdown
---
tipo: fotografia
status: historica
data: AAAA-MM-DD
fonte: 
tags: []
---

# [Nome] — AAAA-MM-DD

> [!important] Retrato histórico
> Este é o estado em AAAA-MM-DD e não muda mais. O estado atual está em [[Nome atual]].
```

A **Decisão** do dia linka a fotografia do dia. Assim, cada decisão fica amarrada ao retrato exato da situação em que foi tomada.

## Template — Aula

```markdown
---
tipo: aula
disciplina: 
professor: 
data: 
status: rascunho
tags: [aula]
---

# [Disciplina] — Aula [n]

## Tema da aula
> Assunto central, em uma frase.

## Conceitos e definições
## Raciocínio
> Como os conceitos se conectam.
## Exemplos e casos
## Dúvidas que ficaram
- [ ] 
## Conexões
- [[ ]] — por quê
```

## Template — Projeto

```markdown
---
tipo: projeto
status: ativo
inicio: 
tags: [projeto]
---

# [Nome do projeto]

## Problema
> O que está errado hoje, com número se possível.
## Objetivo
> Como fica quando estiver resolvido. Mensurável.
## Hipótese
## Plano
- [ ] 
## Métricas
| Métrica | Antes | Meta | Atual |
|---|---|---|---|
## Decisões
- [[Decisão — AAAA-MM-DD — assunto]] — o que decidiu
## Aprendizados
```

## Template — Livro

```markdown
---
tipo: livro
autor: 
status: lendo
tags: [livro]
---

# [Título] — [Autor]

## Por que peguei este livro
## Ideias que mudaram algo em mim
> Não resuma o livro. Registre o que mudou de opinião.
## Trechos
## Onde aplico
- [[ ]] — em que caso concreto
```

## Template — Captura rápida

Fica numa pasta `Inbox/` e é processado na revisão semanal.

```markdown
---
tipo: captura
data: 
status: bruto
---

# [primeira frase que vier]

## O que é
## Por que guardei
## Para onde vai
> Área e nota de destino, definido na revisão semanal.
```
