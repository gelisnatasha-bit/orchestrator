---
name: create-account-repo
description: Creates a new GitHub repository under gelisnatasha-bit from the orchestrator template, copying account rules. Use when the user asks to create a new repo, project, or GitHub repository for this account.
---

# Создать репозиторий аккаунта

Новые репозитории аккаунта https://github.com/gelisnatasha-bit всегда появляются из этого оркестратора, уже с общими правилами.

## Куда класть

Путь: `G:\Projects\personal\<имя-репо>`

Не клади проекты на диск C — там мало места.

## Шаги

1. Уточни имя репозитория, если его нет. Предложи простое имя латиницей, без пробелов.
2. Создай папку `G:\Projects\personal\<имя>`.
3. Скопируй **всё содержимое** `templates/new-repo/` в эту папку (включая `.cursor/rules/`, `.cursor/commands/`, `.cursor/skills/`).
4. Сразу вызови `move_agent_to_root` на новую папку — до любых правок и установки зависимостей.
5. Сделай `git init`, ветка `master`.
6. Создай репозиторий на GitHub в аккаунте `gelisnatasha-bit` (приватный, если пользователь не сказал иное).
7. Добавь remote: `git@github.com-personal:gelisnatasha-bit/<имя>.git`
8. Добавь файлы проекта по задаче пользователя, но **не удаляй** скопированные правила.
9. Коммить и пушь только если пользователь явно попросил.

## Git

На этой машине личный GitHub ходит через SSH-хост `github.com-personal`, не через обычный `github.com`. Так подставляется личный ключ.

## После создания

Напомни: в новом репо уже лежат правила «технический уровень» и gitflow (worktree на фичу, `/Готово` вливает в `master`, без PR).
