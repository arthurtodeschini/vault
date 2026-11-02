# Estratégia de links entre notas

> Esta é a parte que decide se o vault vira conhecimento ou vira bagunça. Trate com o mesmo peso da estrutura de pastas.

## O problema

O Obsidian torna o link tão fácil (`[[assim]]`) que as pessoas linkam por reflexo. Duas notas citam "vendas" → liga uma na outra. Em três meses, o grafo de notas está lindo, tudo aponta para tudo, e ele não diz absolutamente nada.

**Link sem aplicação é ruído.** Ruído em quantidade suficiente destrói o valor dos links que importam.

## A regra única

**Todo link carrega a razão dele, escrita ao lado.**

```markdown
[[Nome da nota]] — por que essa nota importa aqui
```

Teste prático: se a pessoa não consegue escrever essa meia linha, o link não deve existir. Sem exceção, sem "depois eu explico".

## Os três tipos de link que valem a pena

### 1. Origem — "de onde isso veio"

Conecta uma ideia à fonte que a gerou. É o link mais fácil de criar e o mais útil meses depois, quando a pessoa não lembra de onde tirou aquilo.

```markdown
· origem [[Aula 04 — Estrutura de Capital]]
```

### 2. Aplicação — "onde eu uso isso"

Conecta um conceito a um caso concreto que existe em outra nota. É o link que transforma teoria em decisão, e o mais raro de encontrar em vaults abandonados.

```markdown
[[Projeto de precificação]] — usei esse modelo pra definir a faixa de preço
```

### 3. Tensão — "isso discorda daquilo"

Conecta notas que se contradizem ou se limitam mutuamente. É o link mais valioso e quase ninguém faz, porque exige ter lido as duas notas com atenção.

```markdown
[[Nota sobre delegação]] — contradiz isso quando o time tem menos de 10 pessoas
```

## O que não linkar

- **Notas que só compartilham tema.** Isso é trabalho de tag, não de link.
- **Notas que "um dia" vão se conectar.** Se a conexão ainda não existe, o link também não deveria.
- **Listas de "notas relacionadas" no fim da página**, com dez links e nenhuma explicação. É o formato mais comum de bagunça.
- **Links para notas que não existem**, em volume. Um ou outro como marcador de algo a escrever é aceitável; dezenas viram um vault cheio de becos sem saída.

## Tag ou link?

| | Serve para | Exemplo |
|---|---|---|
| **Tag** | Filtrar um conjunto amplo de notas | `#aula`, `#vendas`, `#livro` |
| **Link** | Uma relação específica entre duas notas | `[[Aula 04]] — de onde saiu esse conceito` |

Quem usa tag no lugar de link acaba com um vault que **filtra bem e não pensa**. Quem usa link no lugar de tag acaba com um grafo ilegível. Os dois têm função e não competem.

## Backlinks: a parte que dá o retorno

O Obsidian mostra automaticamente, no rodapé de cada nota, todas as notas que apontam para ela. Isso significa que **um link bem feito paga duas vezes**: na nota onde foi escrito, e na nota de destino, sem esforço nenhum.

É por isso que a razão do link importa tanto. Quando a pessoa abrir a nota de destino meses depois, ela vai ver uma lista de notas que a citaram — e a razão escrita ao lado é o que faz essa lista ser útil em vez de ser um monte de nomes.

## Onde o Claude entra

Peça ao Claude:

- "olha essas notas novas e me diz o que conversa com o que eu já tenho"
- "tem alguma nota minha que contradiz esta aqui?"
- "quais notas minhas ficaram órfãs, sem nenhum link?"

**Mas a decisão de linkar é da pessoa, e a razão do link tem que ser escrita por ela.** Link sugerido e aceito no automático é como link nenhum — reconstrói a mesma bagunça, só que mais rápido.

## O momento de linkar

Não é na hora de criar a nota — nessa hora a pessoa está capturando, e parar para procurar conexões trava o fluxo.

**É na revisão semanal.** Dez minutos, com as notas da semana abertas, perguntando de cada uma: *isso conversa com alguma coisa que eu já tenho?* É o exercício que faz o vault virar cérebro, e é a única parte do ritual que não pode ser pulada.
