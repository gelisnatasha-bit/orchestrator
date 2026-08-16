# Правила аккаунта gelisnatasha-bit

Источник правды для всех будущих репозиториев. Cursor-копии лежат в `.cursor/rules/` и в `templates/new-repo/.cursor/rules/`.

При добавлении правила:

1. Создай файл в этой папке.
2. Сделай `.mdc` копию в `.cursor/rules/` (`alwaysApply: true`, если правило общее).
3. Скопируй то же `.mdc` в `templates/new-repo/.cursor/rules/`.
4. Если правило должно действовать даже до открытия проекта — добавь его ещё как user rule в Cursor.

| № | Правило | Суть |
|---|---------|------|
| 1 | [technical-level.md](technical-level.md) | Подробные объяснения простыми словами |
| 2 | [gitflow.md](gitflow.md) | Фича = ветка + worktree; «Готово» мержит в master, без PR |
| 3 | [code-comments.md](code-comments.md) | Весь код комментировать и документировать |
