# Vitrine de Projetos — Fábrica

Workspace-mãe da maratona de 40 projetos de portfólio (GitHub: `dblzroch`).
Aqui vivem o planejamento e as ferramentas — não os projetos em si.

## Conteúdo

| Arquivo | Para que serve |
|---|---|
| `BACKLOG.md` | Os 40 projetos (10 Python, 10 Flet, 10 Django, 10 FastAPI) com pitch, diferencial, nível e status |
| `CLAUDE.md` | Padrões que o claude-code segue em todo projeto (DoD, estrutura, regras) |
| `scripts/` | Automação: scaffold de projeto novo, geração de índice, sync dos status |
| `site/` | A vitrine em si (GitHub Pages) |

## Pipeline

```
BACKLOG.md  →  novo.sh <stack> <nome>  →  claude-code constrói  →  revisão (lint+testes)  →  push  →  site atualizado
```

## Fluxo de trabalho

1. Escolher o próximo item `⬜` do `BACKLOG.md` e marcá-lo `🔨`.
2. Rodar o scaffold (`scripts/novo.sh`) — cria estrutura, CI, licença, repo no GitHub.
3. Delegar a implementação ao claude-code com `CLAUDE.md` como contexto.
4. Validar: `make lint && make test` verdes + CI verde + README com demo.
5. Marcar `✅` no backlog e regenerar o índice do site.
6. Próximo item. Em lotes de 3-5 quando a stack for a mesma.

## Regra de ouro

Se um projeto não passou no Definition of Done do `CLAUDE.md`, ele fica `🧪` —
nunca vai para `✅` só porque "o código roda".
