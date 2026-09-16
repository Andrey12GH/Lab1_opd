# Памятка по Git

## Ежедневная работа

```text
git status
git diff
git add <path>
git commit -m "краткое описание изменения"
git push
```

`git status` показывает состояние рабочей области и индекса. `git diff` помогает проверить содержание изменений до фиксации.

## История и восстановление

```text
git log --oneline --graph --decorate
git show <commit>
git restore --source=<commit> -- <path>
```

Команда `git show` выводит содержимое и метаданные выбранного коммита. `git restore --source` восстанавливает конкретный файл из указанной версии без перемещения всей ветки.

## Синхронизация с GitHub

```text
git fetch origin
git pull --ff-only
git push -u origin <branch>
```

`git fetch` загружает сведения об удалённых изменениях, не затрагивая рабочую ветку. Параметр `--ff-only` запрещает `pull` создавать неожиданный merge-коммит. Ключ `-u` связывает локальную ветку с удалённой при первой публикации.
