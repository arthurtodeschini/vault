---
name: vault-de-conhecimento
description: Monta um vault de conhecimento no Obsidian do zero absoluto — da instalação do Obsidian e da sincronização até áreas, templates, diagramas, links e o ritual de uso com o Claude. Ative quando alguém disser "quero montar meu vault", "quero começar no Obsidian", "me ajuda a organizar minhas anotações", "não sei onde guardar minhas notas", ou compartilhar uma pasta vazia ou bagunçada. Também revisa um vault que já existe.
---

# Montar um Vault de Conhecimento (Obsidian + Claude)

## O que esta skill faz

Guia uma pessoa, **do zero absoluto**, a montar um vault de Obsidian que funciona no dia a dia. Do zero quer dizer que ela pode nunca ter ouvido falar de Obsidian nem de Markdown e hoje anotar no Word, no app de notas do celular ou num caderno.

O princípio que orienta tudo:

> Uma área do vault só sobrevive se tiver um **gatilho externo** que dispara a criação da nota. Área que depende só de disciplina ("vou anotar quando der") vira pasta vazia com um template caprichado dentro.

**🚫 Nenhuma área entra na estrutura sem um gatilho nomeado.** Se a pessoa não consegue completar *"toda vez que ______ acontece, eu crio uma nota"*, a área não é criada.

Isso vale até para o que é importante. Importância não é gatilho. É comum a área mais importante da vida da pessoa (o trabalho, por exemplo) morrer no vault porque as notas dela nasciam de "quando eu fizer uma análise", e não de um evento que se repete.

## Arquivos de referência

Leia cada um **quando chegar na etapa que o usa**, não antes:

| Arquivo | Conteúdo | Etapa |
|---|---|---|
| `referencias/instalacao.md` | Tutorial de instalação passo a passo, sincronização, configurações, conexão com o Claude, problemas comuns | 0.1 |
| `referencias/estrutura-e-readme.md` | Modelo de estrutura, as três categorias de permissão, moldes de README e CLAUDE.md | 1, 2, 7 |
| `referencias/vocabulario.md` | Valores padrão de `tipo` e `status`, nomes de arquivo | 0.2, 2 |
| `referencias/templates.md` | Moldes: Conteúdo, Evento, Decisão, Nota viva + Fotografia, Aula, Projeto, Livro, Captura | 3, 4 |
| `referencias/diagramas.md` | Quando e como fazer diagramas SVG, regras de legibilidade | 4 |
| `referencias/entradas.md` | As formas de alimentar o vault e como juntar várias fontes numa nota | 4, 6 |
| `referencias/links.md` | Estratégia de links: tipos, o que não linkar, tag × link, backlinks | 5 |
| `referencias/perguntas-em-aberto.md` | O índice de Perguntas em Aberto | 7 |

---

## Como conduzir

**Tom:** conversa, não formulário. **Uma pergunta por vez**, esperando a resposta. Nada de jargão ("PKM", "Zettelkasten", "PARA", "MOC"). Se precisar do conceito, explique com as palavras da pessoa.

**Ritmo:** não despeje as etapas de uma vez. Faça uma, mostre o resultado e siga. Para quem começa do zero, o caminho completo leva de 40 a 60 minutos. Se a pessoa tiver pouco tempo, divida em duas sessões:
- **Sessão 1:** instalação, entrevista, estrutura e primeira nota (Etapas 0 a 4).
- **Sessão 2:** links, ritual e as camadas avançadas (Etapas 5 a 7).

**Regra de ouro:** a pessoa tem que sair da primeira sessão com **uma nota real** dentro do vault, de preferência com um diagrama. Estrutura vazia não convence ninguém a voltar amanhã.

**Verifique, não pergunte:** se você consegue olhar (listar a pasta, abrir um arquivo), olhe. Só pergunte o que não dá pra ver.

---

## Etapa 0 — Descobrir onde a pessoa está

1. Existe uma pasta conectada nesta sessão? Se sim, liste o conteúdo dela.
2. Pergunte só o que não dá pra ver: "você já tem o Obsidian instalado?"
3. Classifique em um dos quatro cenários:

| Cenário | Sinal | Por onde começar |
|---|---|---|
| **A — Zero absoluto** | Sem Obsidian, sem pasta | Etapa 0.1 (tutorial completo) |
| **B — Pasta vazia** | Obsidian instalado, pasta conectada e vazia | Etapa 0.1, só os Passos 5 e 7, depois Etapa 1 |
| **C — Notas soltas** | Arquivos sem estrutura, ou notas em outro app | Etapa 1, com inventário do que já existe |
| **D — Vault já estruturado** | Pastas organizadas e em uso | Etapa 0.2 — revisão |

No cenário C, **leia o que já existe antes de propor qualquer estrutura**. As áreas certas costumam estar escondidas no que a pessoa já escreveu.

### Etapa 0.1 — Instalação (cenário A)

Siga `referencias/instalacao.md`, **um passo por vez, com confirmação**. Em resumo: explicar o que é o Obsidian → decidir a sincronização (computador e celular) → instalar → criar a pasta e abrir como vault → tour de Markdown → quatro ajustes nas configurações → conectar a pasta ao Claude e testar ao vivo.

Só siga para a Etapa 1 quando a pasta estiver conectada e o teste do último passo tiver funcionado.

### Etapa 0.2 — Revisão de um vault existente (cenário D)

Quem já tem estrutura não precisa recomeçar. Precisa de um diagnóstico honesto, **com números**. Nesta ordem:

1. **Mapeie o que existe.** Pastas, número de notas em cada uma e a data da última modificação por pasta.
2. **Identifique as pastas mortas.** Zero ou uma nota, ou nada novo há mais de um mês. Diga isso com o número; é o dado mais útil que a pessoa vai receber.
3. **Aplique o teste do gatilho retroativamente** (Etapa 1) em cada pasta viva e morta. Quase sempre a pasta morreu por falta de gatilho, não de vontade.
4. **Compare o README com a realidade.** É o problema mais comum depois de alguns meses:
   - O README cita templates ou pastas que não existem mais?
   - Existem pastas ou templates que o README não cita?
   - Existem templates espalhados fora da pasta `Templates`?
   - As convenções do README contradizem o que está sendo feito?
5. **Audite o vocabulário.** Liste todos os valores distintos de `tipo:` e `status:` usados nas notas. Se a mesma coisa aparece escrita de vários jeitos (`Concluído`, `concluída`, `fechado`), proponha unificar com `referencias/vocabulario.md`.
6. **Compare com o modelo desta skill** e proponha melhorias, nesta ordem de prioridade:
   - Áreas são domínios de vida ou viraram assuntos? (Etapa 1)
   - O README está fiel à realidade, com gatilhos, permissões e vocabulário? (Etapa 2)
   - Os templates cobrem o que a pessoa de fato produz (eventos, decisões, estado atual)? (Etapa 3)
   - As notas usam diagramas onde o conteúdo tem estrutura? (`referencias/diagramas.md`)
   - Os links têm razão escrita, ou há notas órfãs? (Etapa 5)
   - Existe um ritual semanal marcado? (Etapa 6)
7. **Não reorganize nada sem autorização.** Proponha, explique o porquê e espere o "pode fazer". Mexer na estrutura de um vault em uso quebra links e afasta a pessoa.

Fecho da revisão: **três ações concretas**, não uma lista de vinte.

---

## Etapa 1 — Descobrir as áreas (entrevista)

**Não ofereça uma estrutura pronta.** As áreas têm que sair da vida real da pessoa.

Uma pergunta por vez:

1. "Se eu olhasse sua semana passada hora por hora, em que 3 ou 4 coisas seu tempo foi embora?"
2. "Em qual dessas você já produz alguma coisa escrita hoje, mesmo que bagunçada? (relatório, resumo de aula, planilha, anotação no celular)"
3. "O que você consome que te faz querer anotar? Aula, evento, podcast, livro, post, conversa?"
4. "Tem alguma decisão que se repete na sua vida e que você tomaria melhor se tivesse o histórico das anteriores? (investimentos, contratações, compras grandes, escolhas de projeto)"
5. "Onde suas anotações estão hoje?" (para planejar a migração)

**Como ler as respostas:** áreas são **domínios de vida**, não assuntos. "Trabalho" é área. "Marketing" é assunto, vira nota dentro de Trabalho. Se a pessoa listar 7 áreas, force a escolha de 3. Um vault com 3 áreas vivas vale mais que um com 8 mortas.

Depois de propor as 3 áreas, aplique **o teste do gatilho** em cada uma:

> "Complete: toda vez que ______ acontece, eu abro o Obsidian e crio uma nota."

- Evento concreto e recorrente ("toda vez que termino uma aula", "toda vez que vou a um evento", "toda vez que compro ou vendo um investimento") → a área entra.
- "Quando eu tiver tempo", "quando lembrar", "quando for importante" → **a área não entra**. Explique sem suavizar: pasta sem gatilho fica vazia. Ofereça guardar a ideia num arquivo `Talvez depois.md`.

**Os gatilhos que mais sustentam um vault:**
- **Consumo estruturado:** aula, palestra, evento, curso, livro, post que ensinou algo. São externos e frequentes.
- **Decisões:** toda vez que a pessoa decide algo relevante e repetível. É o gatilho mais subestimado e o que gera as notas mais valiosas a longo prazo.
- **Mudança de estado:** fechamento do mês, atualização da carteira, revisão de metas.

Os mais frágeis são os de **produção espontânea** (diário, ideias soltas). Se a pessoa quiser um deles, exija um gatilho ainda mais concreto, como uma hora fixa na agenda.

Se a pessoa travar e não conseguir nomear as áreas, use o modelo de `referencias/estrutura-e-readme.md`, só como inspiração.

---

## Etapa 2 — Criar a estrutura + o README

Crie as pastas das áreas aprovadas, a pasta `Templates` e, na raiz, um `README.md` que funciona como a **constituição do vault**: estrutura, gatilhos, permissões, vocabulário (`referencias/vocabulario.md`) e convenções.

**Permissões:** pergunte área por área qual destas três categorias ela é:

- 🔒 **Só eu escrevo:** o Claude lê e sugere, mas não cria nem edita. Diário, reflexões, valores, resenhas pessoais.
- 📝 **Claude estrutura, eu penso:** o Claude transforma o material bruto da pessoa em nota, mas as seções de opinião e aplicação ficam marcadas como `> [!question] Leitura do Claude — pra validar` até a pessoa reescrever com as próprias palavras. Aulas, palestras, eventos, decisões.
- 🔓 **Claude escreve e edita:** livre. Projetos, análises, notas de acompanhamento.

A 📝 existe porque a maior parte do que se anota é consumo: proibir o Claude ali faz o vault não crescer, e liberar tudo faz a pessoa terminar com um arquivo organizado e nenhum pensamento próprio. **O Claude faz a estrutura, a pessoa faz o julgamento.** O Claude nunca escreve a aplicação em primeira pessoa como se fosse da pessoa.

Explicação completa e molde do README em `referencias/estrutura-e-readme.md`.

---

## Etapa 3 — Templates (comece com no máximo 2)

Só crie template para tipo de nota que a pessoa **já produz hoje**, com nome e recorrência. Template para nota hipotética é a forma mais rápida de gerar pasta vazia.

Pergunte: "Qual tipo de nota você vai escrever pelo menos uma vez por semana, ou toda vez que [gatilho da Etapa 1] acontecer?"

Escolha os 2 primeiros no catálogo de `referencias/templates.md`:

| Template | Use quando o gatilho for... |
|---|---|
| **Conteúdo** | palestra, post, podcast, vídeo, curso, artigo (costuma ser o mais usado) |
| **Evento** | evento, imersão ou curso com várias palestras ou módulos |
| **Decisão** | decisão relevante e repetível (investimento, contratação, preço, projeto) |
| **Nota viva + Fotografia** | algo com um "estado atual" que muda (carteira, orçamento, metas, funil de clientes) |
| **Aula** | aula de faculdade ou curso com disciplina e sequência |
| **Projeto** | projeto com começo, meta e fim |
| **Livro** | leitura |
| **Captura rápida** | coisas que chegam sem forma e são processadas depois |

Os outros entram depois, **quando o gatilho deles aparecer de verdade**.

---

## Etapa 4 — A primeira nota real (não pule)

É a etapa que faz a pessoa voltar amanhã. Peça material de verdade, agora:

> "Me manda alguma coisa que você quer virar nota: a foto de uma anotação do caderno, as fotos dos slides de uma palestra, um PDF, o print de um post que te fez pensar, ou só me conta uma aula que você teve essa semana."

1. Transforme no template certo e salve na área certa.
2. **Se o conteúdo tem estrutura** (etapas, ciclo, matriz, funil, comparação), **faça o diagrama** e embuta na nota, seguindo `referencias/diagramas.md`. Para a maioria das pessoas, ver um framework virar um diagrama limpo dentro da própria nota é o momento em que o vault "clica".
3. Peça para a pessoa abrir a nota no Obsidian e conferir.
4. **Mostre o que acabou de acontecer:** ela mandou material bruto e saiu uma nota estruturada, visual e pesquisável.

Mostre pelo menos duas das formas de entrada de `referencias/entradas.md`: a versatilidade da entrada é o que derruba a barreira de "não tenho tempo de digitar".

---

## Etapa 5 — Conectar as notas

Uma nota isolada é um arquivo. O que transforma o vault em conhecimento são os **links**, e é aí que a maioria dos vaults vira bagunça: linkar por assunto compartilhado faz tudo apontar para tudo.

**A regra:** todo link carrega a razão dele, escrita ao lado.

```markdown
[[Nome da nota]] — por que essa nota importa aqui
```

Se a pessoa não consegue escrever essa meia linha, o link não deve existir. Os três tipos que valem a pena são **origem**, **aplicação** e **tensão**. Detalhes, exemplos e o que não linkar estão em `referencias/links.md`.

**A decisão de linkar é da pessoa.** O Claude sugere conexões; link aceito no automático é como link nenhum. O momento de linkar é a revisão semanal, não a captura.

Faça agora, ao vivo: pegue a nota da Etapa 4 e encontre pelo menos **um** link com razão explícita. Se ainda não há outra nota, explique a regra e marque para a primeira revisão semanal.

---

## Etapa 6 — O ritual

Estrutura sem ritual é decoração. Feche com três coisas concretas:

1. **Gatilho por área**: já definido, agora escrito no README.
2. **Revisão semanal de 10–15 minutos**, com dia e hora marcados. Nela:
   - ler o que entrou na semana;
   - criar os links que faltaram;
   - reescrever com as próprias palavras as seções "Leitura do Claude — pra validar";
   - **conferir se o README ainda descreve o vault** (pastas, templates, vocabulário);
   - perguntar ao Claude "o que dessas notas conversa entre si?".
3. **A primeira ação de amanhã**, em uma frase concreta: *"amanhã, depois da aula de Finanças, você tira foto do caderno e me manda."*

Sem data e hora, a revisão semanal não acontece. Insista nisso. Feche mostrando o "fluxo de mão dupla" de `referencias/entradas.md`: é o que dá vontade de alimentar o sistema.

---

## Etapa 7 — As duas camadas que fazem a diferença

Só depois que o básico estiver de pé.

- **`CLAUDE.md`** na raiz: quem a pessoa é, seus domínios, projetos ativos e preferências. É o que faz o Claude entender o vault em vez de só ler arquivos. Molde em `referencias/estrutura-e-readme.md`.
- **Índice de Perguntas em Aberto**: toda provocação que um conteúdo gera vira uma nota própria com `status: aberta` e é alimentada até virar decisão. É o que transforma captura em pensamento. Ver `referencias/perguntas-em-aberto.md`.

---

## Erros que esta skill existe para evitar

| Erro | O que acontece | Como evitar |
|---|---|---|
| Pular a instalação guiada | A pessoa trava no primeiro passo e desiste | Etapa 0.1, um passo por vez, com confirmação |
| Vault sem sincronização | Não abre no celular, não sobrevive ao HD | `instalacao.md`, Passo 2 |
| Criar área sem gatilho | Pasta vazia em 3 semanas | Teste do gatilho, sem exceção |
| Confundir importância com gatilho | A área mais importante morre | "Toda vez que ___ acontece" com evento recorrente |
| Estrutura por assunto | Toda nota cabe em 3 lugares, nenhuma é arquivada | Áreas = domínios de vida |
| Muitos templates no começo | Template vira burocracia | Máximo 2; os outros entram com o gatilho |
| Claude pensando pela pessoa | Arquivo organizado, nenhum pensamento novo | Categoria 📝 e "Leitura do Claude — pra validar" |
| Framework só em texto | Ninguém relê | Diagrama embutido onde o conceito aparece |
| Diagrama transparente | Ilegível no tema escuro | Fundo claro próprio em todo SVG |
| Vocabulário solto | O mesmo status escrito de vários jeitos, filtro inútil | Vocabulário padrão no README |
| Linkar por tema | Tudo aponta pra tudo | Todo link com razão escrita |
| Sobrescrever o histórico | Perde-se o que se sabia na época | Nota viva + fotografia; Decisão com "o que eu pensava antes" |
| Sair sem nota nenhuma | Ninguém volta pra uma pasta vazia | Etapa 4 é obrigatória |
| README que envelhece | A documentação promete o que não existe | Conferir o README na revisão semanal |
