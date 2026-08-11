# Erarta Studio

Венчур-студия. Здесь живут собственные продукты портфеля. Клиентские проекты вынесены в отдельные организации — так их можно передать заказчику целиком, не распутывая права.

| Организация | Назначение |
|---|---|
| **erarta** | собственные продукты и инфраструктура портфеля |
| **tamleekplus** | клиентский проект Tamleek (real estate, GCC) |
| **reglament-ai** | клиентский проект Регламент Конференции |

---

## Миграция репозиториев, 11 августа 2026

Весь код переехал из личного аккаунта `mankind-engineering` в организации. Причина — приведение к правилам GitHub: личный аккаунт принадлежит одному человеку, командная работа ведётся через организацию, где у каждого участника своя учётная запись и доступ выдаётся точечно через teams.

**Старые адреса продолжают работать.** GitHub ставит постоянные редиректы при переносе: `git clone`, `git fetch`, `git push` и вызовы API по ссылкам вида `github.com/mankind-engineering/<repo>` автоматически ведут в новое место. Ничего не сломается, если где-то остался старый remote — но обновить его стоит.

```bash
git remote set-url origin https://github.com/erarta/<name>.git
```

### Репозитории, сменившие имя

При экстренной миграции в июне 2026 у части репозиториев обрезали доменные суффиксы. При переносе в организацию описательные имена вернули — здесь путаница наиболее вероятна:

| Было в `mankind-engineering` | Стало |
|---|---|
| `app` | `erarta/app.erarta.ai` |
| `aidi` | `erarta/aidi.app` |
| `studio` | `erarta/studio.erarta.ai` |
| `reflecta` | `erarta/reflecta.vision` |
| `archive-app` | `erarta/archive-app.modera.fashion` |
| `ops-dashboard` | `erarta/ops.erarta.ai` |
| `erarta` | `erarta/erarta.ai` |
| `business` | `erarta/business.erarta.ai` |
| `connect` | `erarta/connect.erarta.store` |
| `luna` | `erarta/luna.ai` |

Отдельно: `erarta/aidi` — это **новая** платформа AIDI, а не старая. Прежний `aidi.app` лежит под своим полным именем.

### Репозитории, сменившие только владельца

Имя не изменилось, поменялся адрес организации:

`zer0` · `modera.fashion` · `modera.shop` · `landing.modera.fashion` · `atlas` · `hermes` · `hermes-legacy` · `hermesa-pitch` · `erarta-pitch` · `erarta-ai-pitch` · `forja` · `advocata` · `citia` · `sonora` · `research` · `ops` · `claude-plugins` · `lexica` · `lexara` · `lora` · `lora-research` · `redata` · `mira` · `polaris` · `qa-agent` · `aqarta` · `solara` · `openclaw` · `telegram-proxy` · `homelab` · `pushiistik` · `we-admin` · `we-app` · `gavanskaya-24` · `xiaozhi-esp32` · `itmo-bonus-track` · `itmo-technological-business`

### Клиентские организации

**tamleekplus** — `tamleek` · `tamleek-app` · `tamleek-admin` · `tamleek-board` · `tamleek-hub` · `tamleek-pr-agent`

**reglament-ai** — `niki` · `marina` · `data`

---

## Правила работы

Личные учётные записи не шарятся между людьми — это нарушение условий GitHub и прямой путь к блокировке аккаунта. Каждый участник заходит под собой и получает доступ к нужным репозиториям через team.

Токены не хранятся в `.git/config` и не вписываются в URL remote'ов.
