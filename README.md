# Vault de Conhecimento — skill para o Claude

Uma skill que guia você, **do zero absoluto**, a montar um vault de anotações no [Obsidian](https://obsidian.md) que funciona no dia a dia, com o Claude ajudando a transformar foto do caderno, slides, PDFs e posts em notas organizadas.

Você não precisa saber o que é Obsidian nem Markdown. A skill conduz tudo como uma conversa: instalação, áreas do vault, templates, a primeira nota real, links entre notas e o ritual semanal. Se você já tem um vault, ela também faz uma revisão.

---

## Como instalar (2 minutos)

### 1. Baixe o arquivo

Clique em **[vault-de-conhecimento.zip](vault-de-conhecimento.zip)** e depois no botão de download (ícone de seta ↓, no canto direito da tela).

> Não descompacte. O Claude recebe o `.zip` do jeito que veio.

### 2. Adicione no Claude

No [claude.ai](https://claude.ai) ou no app do Claude para computador:

1. Vá em **Configurações → Capacidades** (*Settings → Capabilities*).
2. Confira se **Skills** está ativado.
3. Clique em **Enviar skill** (*Upload skill*) e escolha o `vault-de-conhecimento.zip`.

> Skills estão disponíveis nos planos pagos do Claude (Pro, Max, Team e Enterprise).

### 3. Use

Abra uma conversa nova e diga:

> **"Quero montar meu vault de conhecimento."**

O Claude ativa a skill sozinho e começa perguntando onde você está.

---

## Usa o Claude Code?

Copie a pasta `vault-de-conhecimento/` para `~/.claude/skills/`:

```bash
git clone https://github.com/arthurtodeschini/vault.git
cp -r vault/vault-de-conhecimento ~/.claude/skills/
```

---

## O que tem aqui

```
vault-de-conhecimento.zip      ← o arquivo para enviar ao Claude
vault-de-conhecimento/         ← o mesmo conteúdo, aberto, para quem quiser ler
├── SKILL.md                   ← o roteiro principal
└── referencias/               ← instalação, templates, links, diagramas etc.
```

## A ideia por trás

> Uma área do vault só sobrevive se tiver um **gatilho externo** que dispara a criação da nota.

Pasta que depende de "vou anotar quando der" vira pasta vazia em três semanas. Por isso a skill só cria uma área quando você consegue completar: *"toda vez que ______ acontece, eu crio uma nota."*
