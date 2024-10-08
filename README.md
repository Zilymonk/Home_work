﻿# Создали Home_work

```sh
echo "# Home_work" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/Zilymonk/Home_work.git
```

Выполнили 6 условий синхронизации репозитория с Github. Необходимо учитывать того, что если это не чужой репозиторий, а именно твой, то не которые условия могут автоматически произойти вследствии не нужности. Такие как *git branch -M maim* и *git remote add origin <имя_ссылки>*.

Добавили текст об **git push -u origin main** через Web браузер.

# Что такое Git pull & Git push
```sh
git pull
git push
```
Команда *git pull* используется для извлечения и загрузки содержимого из удаленного репозитория и немедленного обновления локального репозитория этим содержимым. Слияние удаленных вышестоящих изменений в локальный репозиторий — это обычное дело в процессе совместной работы на основе **Git**. Команда *git pull* на самом деле представляет собой комбинацию двух других команд: *git fetch и git merge*.

*Git push* — это одна из консольных команд **Git**. Она позволяет передать изменения из локального репозитория (набора файлов из папки .git) в удаленный. Разработчики используют эту команду в следующих целях:
1. Добавить новый функционал в основную ветку.
2. Исправить баг.
3. Закрыть уязвимость в коде и др.

# Основная функция Git merge
```sh
git merge
```
Команда *git merge* выполняет слияние отдельных направлений разработки, созданных с помощью команды *git branch*, в единую ветку.

Обратите внимание: все приведенные ниже команды выполняют слияние в текущую ветку, в то время как целевая ветка остается без изменений. Поэтому команда *git merge* часто используется в сочетании с командами:
1. **git checkout** (для выбора текущей ветки).
2. **git branch -d** (для удаления устаревшей целевой ветки).

# Для чего нужен Pull request в Github?
```sh
pull request
```

**Pull request** — это заявка на слияние кода из разных веток. В процессе слияния *Git* создаст коммит и покажет все изменения в файле кода: добавленные до разветвления строки подсветятся *зеленым цветом*, удаленные — *красным*. Так каждый из разработчиков и менеджер проекта увидят, что произошло с кодом после совместной работы над коммитом. Перед окончательным слиянием (*merge*) все разработчики должны просмотреть изменения кода (*code review*) и принять их.