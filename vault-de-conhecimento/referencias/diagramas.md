# Diagramas

Diagramas são parte central do vault, não enfeite. **Framework em parágrafo raramente é relido; framework em diagrama é.** Ofereça diagrama sempre que o conteúdo tiver estrutura visual.

## Quando fazer

| O conteúdo tem... | Diagrama |
|---|---|
| etapas em sequência | fluxo com setas |
| algo que se retroalimenta | ciclo |
| dois eixos de decisão | matriz 2×2 ou 3×3 |
| níveis ou hierarquia | pirâmide ou degraus |
| afunilamento (leads, vendas) | funil |
| comparação entre opções | colunas lado a lado |
| uma fórmula ou equação de negócio | blocos com operadores |

**Não faça** diagrama de ideia que é só texto corrido, nem diagrama que repete um parágrafo que já diz o mesmo. O diagrama **substitui** a explicação longa; o texto ao redor fica curto.

## Como fazer

1. Gere um arquivo **SVG** e salve **na mesma pasta da nota**.
2. Nome: `[Nota ou autor] - [Conceito] - diagrama.svg`.
3. Embuta **no ponto da nota em que o conceito é explicado**, não no fim:
   ```markdown
   ![[Autor - Conceito - diagrama.svg|780]]
   ```
4. Quando o visual original importa (o slide de uma palestra, um quadro na lousa), guarde também a foto ao lado: `[Nota] - [Conceito] - foto.png`.

## Regras de legibilidade

- **Fundo próprio, sempre.** O Obsidian é muito usado em tema escuro. SVG com fundo transparente e texto escuro fica ilegível. Comece todo SVG com um retângulo de fundo claro cobrindo a área inteira (ex.: `<rect width="100%" height="100%" rx="12" fill="#faf8f4"/>`).
- Fonte sem serifa do sistema (`Helvetica, Arial, sans-serif`), tamanho mínimo 14.
- Título no topo. Pouco texto: palavras-chave, não frases.
- Paleta de 3 a 5 cores, **a mesma em todo o vault**. Na primeira vez, combine a paleta com a pessoa e registre no README.
- Fidelidade à fonte: se o diagrama reproduz o modelo de alguém, mantenha os nomes e a estrutura originais e cite a origem na nota.

Depois de criar, peça para a pessoa abrir no Obsidian e confirmar que está legível.
