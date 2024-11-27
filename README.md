# Git Cheatsheet

## Основные команды Git

- `git init` — инициализация нового локального репозитория.
- `git clone <url>` — клонирование удалённого репозитория.
- `git add <file>` — добавление файла в область подготовленных файлов (staging area).
- `git commit -m "сообщение"` — создание коммита с описанием изменений.
- `git push` — отправка изменений в удалённый репозиторий.
- `git pull` — получение и интеграция изменений из удалённого репозитория.

## Регистрация на GitHub

- Зарегистрируйтесь на сайте [GitHub](https://github.com/).
- Создайте новый репозиторий.
- Скопируйте его на локальный компьютер# git-cheatsheet

## Хеши в Git
- Каждый коммит в Git идентифицируется уникальным хешем, который создаётся на основе содержимого коммита.
- Хеш вычисляется с помощью алгоритма SHA-1, и результатом является строка из 40 символов.
- Хеш используется для быстрого сравнения файлов и отслеживания изменений в репозитории.
- Команда git log позволяет увидеть хеши коммитов в репозитории.

## git log

- git log — команда для просмотра истории коммитов.
- Выводит список всех коммитов, начиная с самого последнего.
- Каждому коммиту присваивается уникальный хеш и метка времени.
- Полезные флаги:
- `--oneline`: краткая версия истории.
- `--graph`: визуализация ветвления.

## HEAD
- `HEAD` указывает на текущий коммит или ветку.
- Используется для перемещения по истории: `git checkout <commit_hash>`.
- Перемещение назад на один коммит: `git reset --hard HEAD~1`.

## Статусы файлов
- **Untracked**: файл ещё не отслеживается.
- **Modified**: файл изменён.
- **Staged**: изменения добавлены в индекс с помощью `git add`.
- **Committed**: изменения сохранены в репозиторий.
- Схема:
    1. Modified → `git add` → Staged.
    2. Staged → `git commit` → Committed.