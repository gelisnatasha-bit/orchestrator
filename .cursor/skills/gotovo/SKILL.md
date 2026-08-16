---
name: gotovo
description: Finishes a feature without a pull request. Use when the user says Готово, /Готово, or asks to merge the current feature into master/main.
---

# Готово

Алиас **Готово**: влить текущую фичу в основную ветку. Pull request не создавать.

## Шаги

1. Определи репозиторий, ветку фичи и папку worktree. Основная ветка — `master`; если её нет — `main`.
2. Незакоммиченные правки — закоммить (понятное сообщение, без секретов). Хуки не пропускать.
3. `git status` должен быть чистым.
4. В основной папке репо (она на `master`/`main`): checkout основной → `git pull` → `git merge --no-ff` ветки фичи → `git push origin` основной ветки.
5. `git worktree remove` папки фичи, `git branch -d` ветки фичи.
6. `move_agent_to_root` в основную папку, `SetActiveBranch` на основную ветку.

Не вызывай `gh pr create`. Не force-push. Конфликт — остановись и объясни простыми словами.

Подробности: `rules/gitflow.md` в оркестраторе, если этот репозиторий его видит.
