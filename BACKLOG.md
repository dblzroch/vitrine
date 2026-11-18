# Backlog — 40 Projetos Portfólio

Status: `⬜` não iniciado · `🔨` em construção · `🧪` em revisão · `✅` publicado

Legenda de nível: **S** = simples (1-2 dias) · **M** = médio (2-4 dias) · **A** = avançado (4-7 dias)

---

## Bloco 1 — Python puro (CLI, libs, automação)

| # | Nome | Pitch | Diferencial (o que faz olhar duas vezes) | Nível | Status |
|---|------|-------|------------------------------------------|-------|--------|
| 01 | `py-task-cli` | Gerencia tarefas pelo terminal com SQLite | Sync opcional com Todoist, TUI com rich, export Markdown | S | ✅ |
| 02 | `py-file-organizer` | Organiza arquivos por regras declarativas em YAML | Dry-run + undo das últimas N operações, watch mode | S | ✅ |
| 03 | `py-image-batch` | Pipeline de resize/watermark/otimização em lote | Paralelismo com `ProcessPoolExecutor`, relatório HTML de ganho | M | ⬜ |
| 04 | `py-crypto-vault` | Cofre de arquivos por linha de comando (AES-256-GCM) | Derivação Argon2id, formato de arquivo documentado na spec | M | ⬜ |
| 05 | `py-scrape-kit` | Framework de scraping com retry, cache e rate-limit | Suporte a paginação via config, export CSV/JSON/SQLite | M | ⬜ |
| 06 | `py-csv-profiler` | Perfil estatístico de CSV → relatório HTML | Detecção de tipos, outliers, sugestão de schema SQL | M | ⬜ |
| 07 | `py-pdf-toolkit` | Merge, split, OCR e marca d'água de PDFs | OCR via Tesseract, monta PDF pesquisável a partir de scans | M | ⬜ |
| 08 | `py-git-stats` | Analytics de repositórios git locais | Heatmap de commits, bus factor, churn por arquivo | M | ⬜ |
| 09 | `py-net-scan` | Scanner de rede local com dashboard no terminal | Fingerprint de serviços, export para CSV, modo passivo | A | ⬜ |
| 10 | `py-telegram-bot` | Bot de automação pessoal (lembretes, agenda, notas) | Persistência SQLite, agendador APScheduler, deploy Docker | M | ⬜ |

## Bloco 2 — Python + Flet (apps desktop/mobile com UI)

| # | Nome | Pitch | Diferencial | Nível | Status |
|---|------|-------|-------------|-------|--------|
| 11 | `flet-financas` | Controle financeiro pessoal | Categorização automática, gráficos, projeção de saldo | M | ⬜ |
| 12 | `flet-habitos` | Tracker de hábitos com streak | Calendário heatmap, notificações, export CSV | S | ⬜ |
| 13 | `flet-notes` | Notas em Markdown com busca | Busca full-text SQLite FTS5, sincronização opcional | M | ⬜ |
| 14 | `flet-kanban` | Kanban com drag & drop | Persistência SQLite, WIP limit, export board | M | ⬜ |
| 15 | `flet-pomodoro` | Pomodoro com estatísticas | Modo "deep work", histórico de foco, gráfico semanal | S | ⬜ |
| 16 | `flet-estoque` | Controle de estoque | Código de barras, alerta de mínimo, relatório de giro | M | ⬜ |
| 17 | `flet-chat-local` | Cliente de chat para LLM local (Ollama) | Streaming de tokens, salvar conversas, system prompt editável | M | ⬜ |
| 18 | `flet-crypto-panel` | Dashboard de cripto em tempo real | API pública, alertas de preço, gráfico com sparkline | M | ⬜ |
| 19 | `flet-pdv` | PDV / frente de caixa simples | Impressão de recibo, fechamento de caixa, multi-usuário | A | ⬜ |
| 20 | `flet-agenda` | Agenda de clientes (clínicas/salões) | Visão dia/semana, confirmação, financeiro por profissional | A | ⬜ |

## Bloco 3 — Django

| # | Nome | Pitch | Diferencial | Nível | Status |
|---|------|-------|-------------|-------|--------|
| 21 | `django-ecommerce` | Loja virtual completa | Carrinho em sessão, cupons, painel de vendas | A | ⬜ |
| 22 | `django-blog-cms` | CMS de blog em Markdown | Editor, tags, comentários moderados, sitemap/SEO | M | ⬜ |
| 23 | `django-helpdesk` | Help desk com tickets | SLA com prazo, anexos, histórico de status | A | ⬜ |
| 24 | `django-crm` | CRM com pipeline de vendas | Kanban de oportunidades, atividades, previsão de receita | A | ⬜ |
| 25 | `django-lms` | Plataforma de cursos | Aulas em vídeo, progresso, certificado em PDF | A | ⬜ |
| 26 | `django-booking` | Sistema de reservas (hotel/salão) | Conflito de horários, calendário, pagamento fake | M | ⬜ |
| 27 | `django-erp-estoque` | ERP de estoque e compras | Movimentações, fornecedores, relatórios em PDF | A | ⬜ |
| 28 | `django-quiz` | Plataforma de provas e quizzes | Banco de questões, correção automática, ranking | M | ⬜ |
| 29 | `django-financeiro` | Gestão financeira com gráficos | Contas a pagar/receber, fluxo de caixa, Chart.js | M | ⬜ |
| 30 | `django-portfolio-cms` | Portfólio pessoal gerenciável | Admin para projetos, tema escuro, deploy fácil | S | ⬜ |

## Bloco 4 — FastAPI

| # | Nome | Pitch | Diferencial | Nível | Status |
|---|------|-------|-------------|-------|--------|
| 31 | `fastapi-auth-api` | Serviço de autenticação reutilizável | JWT + refresh, RBAC, recuperação de senha, testes >90% | M | ⬜ |
| 32 | `fastapi-url-shortener` | Encurtador de URLs | Analytics de cliques, QR code, expiração | S | ⬜ |
| 33 | `fastapi-ecommerce-api` | API REST de e-commerce | Alembic, paginação por cursor, OpenAPI caprichado | A | ⬜ |
| 34 | `fastapi-realtime-chat` | Chat em tempo real | WebSocket, salas, presença online, histórico | M | ⬜ |
| 35 | `fastapi-ml-serving` | Serviço de inferência de modelos | Versionamento de modelo, batch predict, métricas Prometheus | A | ⬜ |
| 36 | `fastapi-job-queue` | Fila de tarefas assíncronas | Redis, retry com backoff, painel de status dos jobs | A | ⬜ |
| 37 | `fastapi-file-storage` | Serviço de upload de arquivos | Presigned URL, geração de thumbnails, quota por usuário | M | ⬜ |
| 38 | `fastapi-rag-api` | API de RAG sobre documentos | pgvector, ingestão de PDF, citação de fontes na resposta | A | ⬜ |
| 39 | `fastapi-webhook-hub` | Hub de webhooks | Assinatura HMAC, retry agendado, log de entregas | M | ⬜ |
| 40 | `fastapi-analytics-api` | Ingestão e consulta de eventos | Agregações por período, cache, rate-limit por API key | M | ⬜ |

---

## Definition of Done (todo projeto, sem exceção)

1. **README** — badges (CI, licença, Python), descrição de 3 linhas, screenshot/GIF, "como rodar" em < 5 comandos, seção de arquitetura curta.
2. **Testes** — `pytest`, cobertura ≥ 80% no core; nenhum teste quebrado.
3. **Qualidade** — `ruff check` + `ruff format` + `mypy` limpos (configurados no repo).
4. **CI** — GitHub Actions rodando lint + testes em push/PR, badge verde.
5. **Empacotamento** — `pyproject.toml` (uv), `.env.example`, `Makefile` ou `justfile` com `make run/test/lint`.
6. **Licença** — MIT.
7. **Deploy/demo** — Docker quando couber; onde houver UI/API, um caminho de demo público (ou GIF no README).
8. **Commits** — Conventional Commits, histórico legível (o `git log` também é avaliado).
9. **Sem segredos** — nada de chave no repo; `.gitignore` correto desde o primeiro commit.
