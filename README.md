<div align="center">
  <img src="./banner.svg" alt="Дмитрий Пасовец — Senior Backend & AI Engineer" width="100%" />
</div>

<p align="center">
  <a href="https://disk.yandex.by/i/9kgdjL2FKScfIQ"><b>Резюме&nbsp;↗</b></a> &nbsp;·&nbsp;
  <a href="https://www.linkedin.com/in/dimacaptain"><b>LinkedIn&nbsp;↗</b></a> &nbsp;·&nbsp;
  <a href="https://career.habr.com/dimacaptain"><b>Хабр&nbsp;Карьера&nbsp;↗</b></a> &nbsp;·&nbsp;
  <a href="https://t.me/captainDima"><b>Telegram&nbsp;↗</b></a>
</p>

---

**Senior Backend-инженер (Node.js / NestJS), 5+ лет.** Веду бэкенд от архитектуры до прода: highload, платежи и подписки, распределённые транзакции и отказоустойчивость. Последние 3 года — плотно на стыке backend и AI: мультиагентные пайплайны, RAG и LLM-security как ежедневный рабочий инструмент, а не хобби.

**Из практики:**

- Спроектировал **order book** криптобиржи с атомарным матчингом (Redlock + распределённые транзакции), price-time priority и восстановлением стакана при сбоях; нагрузочно протестирован на **10k пользователей**.
- **−80% новых багов** на highload-проекте после перепроектирования флоу (Kafka + Debezium); нашёл и починил баг «вечных подписок» (**2000+**) с восстановлением потерянных транзакций — напрямую спас деньги заказчику.
- Спроектировал **6-слойную защиту от prompt injection** (OWASP LLM Top 10): санитизация вход/выход, LLM risk-scoring, outbound-gate, PII/secret redaction.

---

### Проекты

**Мультиагентная система разработки**
Команды агентов Claude Code (Arch / Dev / QA, пары Main/Rev на разных LLM) в tmux-конвейере: авто-ревью, переключение модельных профилей, дашборд состояния агентов и детерминированный **autoapprove-хук** (Claude Code PreToolUse) с deny-list политикой. Idempotent-инсталляция (symlinks + cron), репозиторий как single-source-of-truth, bats-тесты. Мой основной рабочий инструмент разработки.
`TypeScript` · `tmux` · `Claude Code` · `PreToolUse hooks` · `multi-model routing`

**Квант — распределённый персональный AI-ассистент**
Telegram ↔ Claude Code через CCR с полным доступом к инструментам (веб-поиск, файлы, код, зрение). **Два инстанса** — локальный и облачный (VPS) — с общей **git-памятью** (vault local / cloud / shared, автосинк) и системой из **8 доменных ролей**, мультипользовательский доступ.
`Node.js` · `CCR` · `Claude Code` · `git-based memory` · `MCP`

**Zipper — AI-тьютор для ускоренного обучения**
Next.js 15 + RAG на локальных эмбеддингах (Ollama, bge-m3) и векторном поиске (SQLite + sqlite-vec), Vercel AI SDK. Несколько режимов тьюторинга (сократовский диалог, опрос, mock-экзамен), ingest-конвейер учебных материалов (PDF / EPUB / FB2 + транскрипции лекций), трекинг прогресса освоения.
`Next.js 15` · `TypeScript` · `RAG` · `sqlite-vec` · `Ollama / bge-m3` · `Vercel AI SDK`

---

### Стек

**Языки** — TypeScript · JavaScript (Node.js) · SQL · базово Python
**Бэкенд** — NestJS · Express · Fastify · REST · GraphQL · gRPC · WebSocket · микросервисы
**Архитектура** — Event-Driven · DDD · CQRS · распределённые транзакции · идемпотентность · проектирование под нагрузку
**Данные / очереди** — PostgreSQL · MongoDB · Redis · Kafka · RabbitMQ · BullMQ
**Cloud / DevOps** — Docker · Kubernetes · GitLab CI/CD · AWS · GCP · Nginx
**AI / LLM** — мультиагентные системы · RAG · pgvector / Qdrant · embeddings · MCP · OpenRouter · OWASP LLM Top 10

---

<p align="center">
  <sub>Открыт к senior / lead backend-роли в продукте, где нужен широкий бэкендер, умеющий в AI.<br/>
  Быстрее всего отвечаю в <a href="https://t.me/captainDima">Telegram</a> &nbsp;·&nbsp; dimitricaptain@yandex.by</sub>
</p>
