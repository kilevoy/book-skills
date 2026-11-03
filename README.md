# Скиллы из книг для Claude Code и Codex

Пять книг, превращённых в скиллы. С ними модель отвечает по правилам книги,
а не усреднённо.

| Скилл | Книга | Для чего |
|---|---|---|
| `pishi-sokraschay` | «Пиши, сокращай», Максим Ильяхов и Людмила Сарычева | редактура текстов в инфостиле |
| `voss-negotiation` | «Никаких компромиссов», Крис Восс и Тал Раз | переговоры, торг о цене |
| `mom-test` | «Спроси маму», Роб Фитцпатрик | интервью с клиентами, проверка идеи |
| `goldratt-constraints` | «Цель», Элияху Голдратт и Джефф Кокс | поиск узкого места в бизнесе |
| `atomic-habits` | «Атомные привычки», Джеймс Клир | привычки и регулярность |

## Установка

Claude Code:

```bash
git clone https://github.com/HinkoK/book-skills.git
cp -R book-skills/skills/* ~/.claude/skills/
```

Codex:

```bash
git clone https://github.com/HinkoK/book-skills.git
mkdir -p ~/.agents/skills
cp -R book-skills/skills/* ~/.agents/skills/
```

После копирования перезапусти Claude Code или Codex. Скилл подключается сам,
когда задача подходит под его описание. В Claude Code его можно вызвать и по
имени, например `/pishi-sokraschay`.

## Что внутри скилла

- `SKILL.md`: главные методики книги и указатель по темам
- `chapters/`: конспект каждой главы отдельным файлом, модель читает только нужную
- `glossary.md`: термины книги
- `patterns.md`: приёмы и техники
- `cheatsheet.md`: шпаргалка с правилами

Скиллы собраны инструментом [book-to-skill](https://github.com/virgiliojr94/book-to-skill).

Это конспекты для работы, а не текст книг. Сами книги стоит прочитать целиком.
