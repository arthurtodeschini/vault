# Tutorial de instalação (do zero absoluto)

> Usado na Etapa 0.1 do SKILL.md, no cenário A (sem Obsidian, sem pasta). No cenário B, use só os Passos 5 e 7.

Conduza passo a passo. **Espere a confirmação de cada passo antes do próximo.** Se a pessoa travar, peça um print da tela e oriente a partir dele.

## Passo 1 — Explicar o que é o Obsidian (30 segundos)

Diga algo assim, com suas palavras:

> "O Obsidian é um app de anotações gratuito. A diferença dele é que cada nota é um arquivo de texto comum, guardado numa pasta do seu computador. A pasta é sua, não fica presa num app. Por isso eu (Claude) consigo ler e escrever nas suas notas quando você conecta essa pasta comigo. O Obsidian chama essa pasta de **vault** (cofre)."

## Passo 2 — Decidir onde a pasta vai morar (sincronização)

Isso não é detalhe: é o que faz o vault abrir no celular e sobreviver a um computador roubado ou um HD queimado. Faça **duas perguntas**:

1. "Você usa computador Windows ou Mac?"
2. "Quer ver e escrever notas no celular também? iPhone ou Android?"

Recomende pela tabela abaixo:

| Situação | Recomendação | Por quê |
|---|---|---|
| Só computador | Pasta dentro do serviço de nuvem que a pessoa já usa (Dropbox, Google Drive, OneDrive ou iCloud) | Gratuito, sem configuração extra |
| Mac + iPhone | Pasta no **iCloud Drive** | É o caminho nativo e gratuito do Obsidian no iPhone |
| Windows + iPhone, ou qualquer combinação com Android | **Obsidian Sync** (pago) **ou** só computador por enquanto | O app de celular do Obsidian não abre pastas do Dropbox/Google Drive diretamente; os atalhos gratuitos para isso dão trabalho e quebram com facilidade |
| Quer o máximo de segurança e histórico de versões | Obsidian Sync | Criptografado e com histórico, sem depender de outro serviço |

Seja honesto sobre a troca: celular sem Obsidian Sync só é simples no ecossistema Apple com iCloud. Para quem está começando, **"só no computador por enquanto" é uma resposta perfeitamente boa**. O vault pode ganhar o celular depois.

> ⚠️ Se a pasta ficar no Dropbox, Google Drive ou OneDrive, ela precisa estar **disponível offline** no computador (no Dropbox: "Disponibilizar offline"; no Drive e no OneDrive: "Sempre manter neste dispositivo"). Arquivo "só na nuvem" não aparece direito no Obsidian nem para o Claude.

## Passo 3 — Instalar

1. Entrar em **obsidian.md** e clicar em Download. O site detecta Windows ou Mac.
2. Instalar como qualquer programa. No Mac, arrastar para a pasta Aplicativos.
3. Abrir o Obsidian. Ele mostra uma tela de boas-vindas com opções de vault.

## Passo 4 — Criar a pasta e abrir como vault

1. **Antes**, no explorador de arquivos (Windows) ou no Finder (Mac), criar uma pasta dentro do local escolhido no Passo 2. Sugira um nome simples: `Vault` ou `Conhecimento`.
2. No Obsidian: **"Abrir pasta como vault"** (Open folder as vault) e selecionar essa pasta.
3. Se a pessoa for usar Obsidian Sync: em vez disso, "Criar novo vault" e depois ativar o Sync nas configurações.

Confirme: "o Obsidian abriu com uma barra lateral vazia à esquerda?"

## Passo 5 — Tour de 2 minutos + Markdown básico

Mostre só o essencial:
- **Barra da esquerda:** as pastas e notas (é a mesma pasta que está no computador).
- **Criar nota:** ícone de lápis/papel no topo da barra, ou `Ctrl+N` (Mac: `Cmd+N`).
- **Markdown**, o jeito de formatar no Obsidian. Ensine só cinco coisas e peça para a pessoa testar numa nota chamada `Teste`:

| Escreve | Vira |
|---|---|
| `# Título` | título grande (`##` para subtítulo) |
| `**negrito**` | **negrito** |
| `- item` | lista |
| `[[Nome de outra nota]]` | link para outra nota (a parte mais importante do Obsidian) |
| `![[imagem.png]]` | imagem ou diagrama embutido na nota |

Tranquilize a pessoa: "não precisa decorar. Eu escrevo a maior parte das notas estruturadas pra você; isso é só pra você não estranhar."

## Passo 6 — Quatro ajustes nas configurações

Configurações = ícone de engrenagem ⚙ no canto inferior esquerdo. Faça um por vez:

1. **Arquivos e links → "Usar [[Wikilinks]]"**: ligado.
2. **Arquivos e links → "Atualizar links internos automaticamente"**: ligado. Assim, renomear uma nota não quebra os links para ela.
3. **Arquivos e links → "Local padrão para novos anexos"**: "Mesma pasta do arquivo atual". Assim, imagens e diagramas ficam ao lado da nota que os usa.
4. **Plugins principais → Templates** (em português pode aparecer como "Modelos"): ligar. Depois, nas configurações do plugin, apontar a "pasta de templates" para `Templates` (você cria essa pasta na Etapa 2).

**Não instale plugins da comunidade agora.** É a forma mais rápida de transformar o começo em um projeto de configuração. Se um dia fizer falta, a pessoa instala.

## Passo 7 — Conectar a pasta ao Claude (e testar)

1. A pessoa conecta **essa mesma pasta** ao Claude, no app do Claude para computador, adicionando a pasta à conversa. Sem isso, o Claude não enxerga nada e metade do valor se perde.
2. **Teste ao vivo:** liste o conteúdo da pasta. Você deve ver a nota `Teste` do Passo 5. Depois crie uma nota curta chamada `Olá do Claude.md` e peça para a pessoa conferir se ela apareceu no Obsidian.

Esse teste é o primeiro "uau" da sessão: a pessoa vê uma nota aparecer sozinha no vault dela.

## Problemas comuns na instalação

| Sintoma | Causa provável | Solução |
|---|---|---|
| Nota criada pelo Claude não aparece no Obsidian | O vault aberto e a pasta conectada são pastas diferentes | Confirmar o caminho das duas; no Obsidian, o ícone de cofre no canto inferior esquerdo mostra qual vault está aberto |
| Arquivos aparecem cinzentos ou não abrem | Pasta de nuvem com arquivos "só online" | Marcar a pasta como disponível offline (Passo 2) |
| Nota abre como texto estranho | Arquivo salvo como `.txt` ou `.docx` | Notas do Obsidian são `.md`; converter ou recriar |
| Aparece um aviso de "modo restrito" | Padrão do Obsidian para plugins da comunidade | Pode ignorar; não precisamos de plugins agora |

Só siga quando a pasta estiver conectada e o teste do Passo 7 tiver funcionado.
