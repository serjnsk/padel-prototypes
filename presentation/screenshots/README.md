# Скриншоты для слайдов

Два источника слайдов:

1. **Скриншот сервиса** — когда прототипа нет и он не нужен. Файл кладётся в эту папку вручную, затем переименовывается по схеме `NN-name.png` и вписывается в таблицу ниже.
2. **Прототип** — готовый берётся с опубликованных страниц https://serjnsk.github.io/padel-prototypes/; если его нет, сначала верстается по скриншоту сервиса, деплоится и снимается.

Слайды роадмапа — по структуре «слева текст, справа экран»: текст пишется в деке, скриншот берётся из прототипа.

Скриншоты прототипов снимаются headless Chrome, окно 2000×1100 (для коротких страниц 2000×900). Команда из корня проекта:

```bash
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new --disable-gpu --hide-scrollbars --window-size=1920,1080 --screenshot="$PWD/presentation/screenshots/NN-name.png" "https://serjnsk.github.io/padel-prototypes/prototypes/page.html"
```

Все прототипы кабинета показывают вид организатора (Алексей Мироносицкий, разделы Турниры · Чемпионаты / Лиги · Игроки). Перед съёмкой прототип должен быть задеплоен, чтобы слайд совпадал с тем, что увидят по ссылке.

| Файл | Слайд | Источник |
|---|---|---|
| `01-landing.png` | 1 · Вступление | `prototypes/landing.html` |
| `02-cabinet.png` | 2 · 2.1 Кабинет организатора | `prototypes/tournaments-list.html` |
| `03-wizard-1-basic.png` | 3 · 2.2 Создание турнира, шаг 1 «Основные настройки» | `prototypes/tournament-basic-step.html` |
| `04-wizard-2-type.png` | 4 · 2.2 Создание турнира, шаг 2 «Тип турнира» | `prototypes/tournament-type-step.html` |
| `05-wizard-3-matches.png` | 5 · 2.2 Создание турнира, шаг 3 «Настройки матчей» | `prototypes/tournament-matches-step.html` |
| `06-wizard-4-participants.png` | 6 · 2.2 Создание турнира, шаг 4 «Участники» | `prototypes/tournament-participants-step.html` |
| `07-run-1-applications.png` | 7 · 2.3 Приём заявок, кабинет | `prototypes/tournament-applications.html` |
| `08-run-1-showcase.png` | 8 · 2.3 Приём заявок, витрина | `prototypes/showcase-applications.html` |
| `09-run-2-draw.png` | 9 · 2.3 Жеребьёвка, кабинет | `prototypes/tournament-draw.html` |
| `10-run-2-tv-draw.png` | 10 · 2.3 Жеребьёвка, ТВ-табло | `prototypes/tv-draw.html` |
| `11-run-3-schedule.png` | 11 · 2.3 Расписание, кабинет | `prototypes/tournament-schedule.html` |
| `12-run-3-bracket.png` | 12 · 2.3 Сетка, витрина | `prototypes/showcase-bracket.html` |
| `13-run-3-tv-schedule.png` | 13 · 2.3 Расписание, ТВ-табло | `prototypes/tv-schedule.html` |
| `14-run-4-results.png` | 14 · 2.3 Завершение турнира, витрина | `prototypes/showcase-results.html` |
| `15-roadmap-referee.png` | — · 3.1 Судейство, вариант А, тёмная тема | `prototypes/referee-scoring.html?t=dark`, окно 560×950 при `--force-device-scale-factor=2` |
| `16-roadmap-referee-light.png` | — · 3.1 Судейство, вариант А, светлая тема | `prototypes/referee-scoring.html?t=light` |
| `17-roadmap-referee-b.png` | — · 3.1 Судейство, вариант Б, тёмная тема | `prototypes/referee-scoring-classic.html?t=dark` |
| `18-roadmap-referee-b-light.png` | — · 3.1 Судейство, вариант Б, светлая тема | `prototypes/referee-scoring-classic.html?t=light` |
| `19-roadmap-referee-c.png` | 15 · 3.1 Судейство, вариант В, тёмная тема | `prototypes/referee-scoring-mix.html?t=dark` |
| `20-roadmap-referee-c-light.png` | 15 · 3.1 Судейство, вариант В, светлая тема | `prototypes/referee-scoring-mix.html?t=light` |
| `21-roadmap-tv-live.png` | 16 · 3.2 Табло у корта | `prototypes/tv-live-score.html` |
| `22-roadmap-broadcast.png` | 17 · 3.2 Виджет в трансляции | `prototypes/broadcast-overlay.html` |
| `23-roadmap-brand-tv.png` | 18 · 3.3 Табло в бело-красной схеме | `prototypes/brand-tv-fonbet.html` |
| `24-roadmap-brand-showcase.png` | 19 · 3.3 Витрина в бело-красной схеме | `prototypes/brand-showcase-fonbet.html` |
| `25-roadmap-brand-sponsors.png` | 20 · 3.3 Варианты размещения логотипов | `prototypes/brand-sponsor-variants.html` |
