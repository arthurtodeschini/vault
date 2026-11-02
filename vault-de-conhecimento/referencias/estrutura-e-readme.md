# Estrutura, README e CLAUDE.md

> Usado nas Etapas 1, 2 e 7 do SKILL.md.

## Modelo de estrutura (só para destravar)

Nunca ofereça antes da entrevista da Etapa 1. Use só se a pessoa não conseguir nomear as próprias áreas.

```
📁 Trabalho                🔓 projetos, análises, decisões
📁 Pessoal
   └── Quem Sou            🔒 identidade, valores
   └── Formação
       └── Faculdade       📝 aulas e trabalhos
       └── Livros          🔒 leituras
       └── Cursos & Eventos 📝 palestras, cursos, conteúdos
   └── Finanças            📝 decisões e carteira
   └── Reflexões & Diário  🔒 pensamento próprio
📁 Projetos Próprios       🔓 ideias e negócios fora do trabalho
📁 Templates               🔓 moldes de nota
```

`Templates` é infraestrutura e não conta no limite de três áreas. Cada subpasta de `Pessoal` tem um gatilho distinto (aula, livro, evento, decisão financeira), e é isso que a mantém viva.

**O que observar:** as pastas mais vivas costumam ser as de consumo estruturado (aula, evento, livro) e as de decisão, porque o gatilho é externo. As mais frágeis são as de produção espontânea (diário, ideias soltas), que dependem de disciplina.

---

## As três categorias de permissão

Pergunte área por área qual categoria ela é. Explique as três com exemplos da vida da pessoa:

| Categoria | O que significa | Serve para |
|---|---|---|
| 🔒 **Só eu escrevo** | O Claude lê, sugere conexões e aponta lacunas, mas não cria nem edita | Diário, reflexões, valores, resenhas pessoais: onde escrever é o próprio pensamento |
| 📝 **Claude estrutura, eu penso** | O Claude transforma o material bruto da pessoa (foto do caderno, slides, PDF, áudio) em nota estruturada. As seções de opinião e aplicação ("como isso se aplica ao meu caso") ficam marcadas como `> [!question] Leitura do Claude — pra validar` até a pessoa reescrever com as próprias palavras | Aulas, palestras, eventos, cursos, decisões |
| 🔓 **Claude escreve e edita** | Livre | Projetos, análises, documentação operacional, notas vivas de acompanhamento |

**Por que a categoria 📝 existe:** a maior parte do que as pessoas anotam é consumo (aula, palestra, conteúdo). Proibir o Claude de escrever ali faz o vault não crescer; liberar tudo faz a pessoa terminar com um arquivo bem organizado e nenhum pensamento próprio. A 📝 separa as duas coisas: **o Claude faz a transcrição e a estrutura, a pessoa faz o julgamento.** O Claude nunca escreve a aplicação em primeira pessoa como se fosse da pessoa.

---

## Molde de README.md

Salvar na raiz do vault. É a constituição do vault: estrutura, gatilhos, permissões, vocabulário e convenções.


```markdown
# Vault de Conhecimento — [Nome]

> Última revisão: AAAA-MM-DD (atualizar na revisão semanal)

## Estrutura
📁 [Área 1]   🔓
📁 [Área 2]   📝
📁 [Área 3]   🔒
📁 Templates  🔓

## Gatilhos
| Área | Toda vez que... | ...eu crio uma nota |
|---|---|---|
| [Área 1] | [evento concreto] | [tipo de nota] |

## Permissões
### 🔒 Só eu escrevo
- [áreas] — o Claude lê, sugere conexões e aponta lacunas, mas não cria nem edita sem eu pedir.
### 📝 Claude estrutura, eu penso
- [áreas] — o Claude transforma meu material bruto em nota; seções de aplicação ficam marcadas "Leitura do Claude — pra validar" até eu reescrever.
### 🔓 Claude escreve e edita
- [áreas]

## Templates em uso
| Template | Para |
|---|---|
| [nome] | [gatilho] |

## Vocabulário
[tabela de tipo/status em uso — só os que este vault usa]

## Convenções
- Links: `[[Nome da nota]] — razão do link` (link sem razão não entra)
- Tags: minúsculas, sem acento, com hífen
- Datas: `AAAA-MM-DD`
- Diagramas: SVG com fundo claro, na pasta da nota, paleta: [cores]

## Revisão semanal
[Dia] às [hora]: reler o que entrou, linkar, validar "Leituras do Claude", conferir este README.
```


**Atenção:** o README envelhece rápido. É comum, depois de alguns meses, ele citar templates e pastas que não existem mais e deixar de citar os novos. Por isso ele entra na revisão semanal.

---

## Molde de CLAUDE.md

Salvar na raiz. É o que faz o Claude entender o vault em vez de só ler arquivos soltos.


```markdown
# Memória de trabalho — [Nome]

> Atualizado: AAAA-MM-DD

## Eu
[Nome] — [o que faz]
Domínios: **[Área 1]**, **[Área 2]**, **[Área 3]**

## Contexto por domínio
| Domínio | O que é |
|---|---|
| [Área 1] | [1-2 linhas de contexto real] |

## Projetos ativos
| Projeto | Domínio | Status |
|---|---|---|

## Como trabalhar comigo no vault
- Antes de editar, checar a permissão da pasta no README.
- [preferências de tom, tamanho, idioma]
```
