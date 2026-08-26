# grok-skills

Skills para agentes de IA no formato [Agent Skills](https://agentskills.io) (`SKILL.md` + referências).

Feitas para o Grok, mas copiam para Claude, Cursor e qualquer agente que carregue o spec.

## Skills

| Skill | O que faz | Trigger |
| --- | --- | --- |
| [marketing-social](./marketing-social/SKILL.md) | Ganchos, formatos de post, copy de anúncio e propostas de engajamento | `/marketing`, `/gancho`, cria post, carrossel, reel, thread |
| [meme](./meme/SKILL.md) | Memes virais com Grok Imagine + prompt copy-paste | `/meme`, gera um meme, template |
| [teach](./teach/SKILL.md) | Lições interativas, loops socráticos e maestria | ensina, me explica, lesson |
| [ui-design-styles](./ui-design-styles/SKILL.md) | 10 estilos de UI (glass, bento, brutalism, etc.) | landing, UI kit, glassmorphism |

## Como usar no Grok

1. Copie a pasta da skill para `~/.grok/skills/<nome>/` (ou `.grok/skills/` no workspace).
2. Dispare com as palavras do `description` no frontmatter.
3. O agente lê o `SKILL.md` e, se precisar, os arquivos em `references/`.

## Como usar em outros agentes

Qualquer runtime compatível com Agent Skills:

```
skill-name/
├── SKILL.md
└── references/   # opcional
```

O campo `description` do frontmatter é o trigger. Mantenha-o sem aspas, sem `: ` e sem `< >`.

## Estrutura

```
grok-skills/
├── marketing-social/
│   ├── SKILL.md
│   └── references/
├── meme/
│   ├── SKILL.md
│   └── references/
├── teach/
│   └── SKILL.md
└── ui-design-styles/
    ├── SKILL.md
    ├── styles/
    └── examples/
```

## Licença

MIT. Use, forke e adapte.

Autor: [Guilherme Pimentel](https://github.com/ggampp) · [x.com/ggampp](https://x.com/ggampp)
