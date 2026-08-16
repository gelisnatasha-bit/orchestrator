# Ассистент в orchestrator

Это репозиторий-оркестратор аккаунта https://github.com/gelisnatasha-bit.

## Обязательно

- Следуй правилу технического уровня: подробные объяснения простыми словами (`rules/technical-level.md`).
- Gitflow без PR: фича = ветка `feat/…` и worktree; «Готово» / `/Готово` мержит в `master` (`rules/gitflow.md`). Не создавай pull request.
- Общие правила живут здесь. Новые репозитории этого аккаунта получают копию из `templates/new-repo/` (включая `.cursor/rules`, `.cursor/commands`, `.cursor/skills`).
- Новые проекты создавай в `G:\Projects\personal`, не на диске C. Основная ветка новых репо — `master`.
- Для клонирования и push используй SSH-хост `github.com-personal` (личный ключ), например: `git@github.com-personal:gelisnatasha-bit/ИМЯ.git`.

## Когда просят новое правило

1. Добавь человекочитаемый файл в `rules/`.
2. Добавь `.mdc` в `.cursor/rules/`.
3. Скопируй `.mdc` в `templates/new-repo/.cursor/rules/`, чтобы будущие репо тоже его получили.
4. Если правило глобальное для аккаунта — добавь user rule в Cursor.

## Когда просят новый репозиторий

Читай skill `.cursor/skills/create-account-repo/SKILL.md` и выполняй его целиком.
