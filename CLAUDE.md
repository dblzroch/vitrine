# CLAUDE.md — Padrões da Fábrica de Projetos

Estas regras valem para TODOS os projetos gerados por esta fábrica.
Leia este arquivo antes de escrever qualquer linha de código.

## Objetivo

Cada projeto é uma peça de portfólio público no GitHub (conta `dblzroch`).
O critério de sucesso NÃO é "funciona na minha máquina" — é **um estranho clonar, rodar em menos de 5 comandos e ver valor em 30 segundos**.

## Stack e ferramentas obrigatórias

- **Python 3.12+** gerenciado por **`uv`** (`uv sync`, `uv run`). Nunca `pip install` solto no README.
- Lint/format: **ruff** (`ruff check` + `ruff format`).
- Tipos: **mypy** no modo padrão, com tipagem em toda função pública.
- Testes: **pytest** + `pytest-cov`.
- Configuração de ferramentas sempre dentro do `pyproject.toml` (`[tool.ruff]`, `[tool.mypy]`, `[tool.pytest.ini_options]`).

## Estrutura padrão

```
<nome>/
├── README.md
├── LICENSE               # MIT, ano atual, Diego (dblzroch)
├── pyproject.toml
├── .gitignore
├── .env.example          # se houver config; nunca .env real
├── Makefile              # run, test, lint, fmt
├── .github/workflows/ci.yml
├── src/<pacote>/         # código (layout src)
├── tests/
└── docs/                 # apenas quando houver decisão de arquitetura a explicar
```

## Definition of Done (não entregue nada incompleto)

1. `make test` verde, cobertura >= 80% no core.
2. `make lint` sem erro (ruff + mypy).
3. CI do GitHub Actions verde (lint + testes em push/PR).
4. README com: badges, parágrafo de 3 linhas, screenshot/GIF, "Quickstart" em até 5 comandos, seção curta de arquitetura, licença.
5. `.gitignore` correto desde o primeiro commit.
6. Commits em **Conventional Commits** (`feat:`, `fix:`, `docs:`, `test:`, `chore:`), em português ou inglês — mas consistentes no repo.

## Regras de código

- Type hints em todas as funções públicas; docstring curta (Google style) nas públicas não triviais.
- Sem `print` de debug no código final — use `logging`.
- Trate erro de forma explícita; nada de `except:` nu.
- Funções pequenas; sem classe gigante. Prefira composição.
- Nada de dependência pesada sem justificar no README (diga o porquê da escolha).
- Sem segredo, token ou chave no repositório — jamais.

## README — template mental

```markdown
# <Nome>

> Uma frase do que faz.

[badges: CI | licença | python]

Parágrafo curto: problema, solução, para quem serve.

![demo](docs/demo.gif)

## Quickstart
uv sync
uv run <comando>

## Como funciona
2-4 linhas de arquitetura. Se houver decisão não óbvia, linke docs/adr.

## Testes
make test

## Licença
MIT
```

## Tom

Escreva o README como um dev sênior escreveria: direto, técnico, sem enfeite de marketing.
Português no corpo quando o projeto for claramente PT-BR; termos técnicos em inglês.

## Proibido

- Entregar projeto só com scaffold e TODOs.
- Deixar teste quebrado ou comentado.
- Commit gigante "initial commit" com tudo dentro quando der para separar.
- README genérico de template sem adaptar ao projeto real.