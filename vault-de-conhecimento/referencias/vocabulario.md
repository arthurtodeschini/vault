# Vocabulário padrão

Vault com o mesmo conceito escrito de três jeitos fica impossível de filtrar. Registre este vocabulário no README e **não invente valor novo sem antes adicioná-lo ao README**.

**Regras gerais:** tudo em minúsculas, sem acento, singular, com hífen no lugar de espaço. Datas sempre `AAAA-MM-DD`.

| `tipo` | `status` possíveis | Observação |
|---|---|---|
| `conteudo` | `rascunho` · `pronta` | Campo extra `formato`: `palestra` · `post` · `podcast` · `video` · `curso` · `artigo` |
| `aula` | `rascunho` · `pronta` | |
| `evento` | `em-andamento` · `concluido` | Nota-hub do evento |
| `decisao` | `tomada` · `revisada` | `revisada` = já olhei de volta e registrei o aprendizado |
| `nota-viva` | `ativa` · `arquivada` | Estado atual de algo; é sobrescrita |
| `fotografia` | `historica` | Retrato datado; nunca muda |
| `projeto` | `ativo` · `pausado` · `concluido` | |
| `livro` | `quero-ler` · `lendo` · `lido` | |
| `captura` | `bruto` · `processado` | |
| `pergunta` | `aberta` · `resolvida` | Ver `perguntas-em-aberto.md` |
| `indice` | `ativo` | Notas que só organizam outras |

**Nomes de arquivo:**
- Conteúdo: `Autor - Título`
- Decisão: `Decisão — AAAA-MM-DD — assunto`
- Fotografia: `[Nome da nota viva] — AAAA-MM-DD`
- Diagrama: `[Nota] - [Conceito] - diagrama.svg` · Foto: `[Nota] - [Conceito] - foto.png`
- Sempre descritivos, sem sigla obscura.
