## Git справочник

### Основные команды
git init – инициализировать новый репозиторий.

git clone <url> – склонировать удалённый репозиторий.

git status – проверить состояние файлов (изменённые, добавленные, удалённые).

git add <file> / git add . – добавить файлы в индекс (staging area).

git commit -m "сообщение" – зафиксировать изменения с комментарием.

git push – отправить изменения в удалённый репозиторий.

git pull – получить изменения из удалённого репозитория.

git fetch – загрузить изменения из удалённого репозитория без слияния.

### Ветки (Branches)
git branch – показать список веток.

git branch <name> – создать новую ветку.

git checkout <branch> – переключиться на ветку.

git checkout -b <new_branch> – создать и переключиться на новую ветку.

git merge <branch> – влить изменения из другой ветки.

git rebase <branch> – перебазировать текущую ветку на другую.

### Отмена изменений
git restore <file> – отменить изменения в файле (до git add).

git restore --staged <file> – убрать файл из индекса (после git add).

git reset --hard – отменить все локальные изменения (осторожно!).

git commit --amend – исправить последний коммит.

### История и логи
git log – показать историю коммитов.

git log --oneline --graph – компактный вывод с визуализацией веток.

git diff – показать изменения между файлами.

git show <commit> – показать изменения в конкретном коммите.

### Работа с удалённым репозиторием
git remote -v – показать список удалённых репозиториев.

git remote add <name> <url> – добавить удалённый репозиторий.

git push -u origin <branch> – отправить ветку в удалённый репозиторий (в первый раз).

git push --force – принудительно отправить изменения (осторожно!).


### git config
git config --global user.name "John Doe"\
git config --global user.email johndoe@example.com

## SSH key
- ls -al ~/.ssh - проверка существующих ключей

- ssh-keygen -t ed25519 -C "johndoe@example.com" - генерация ключа

- добавляем ключ в github /settings/keys

- ssh-add ~/.ssh/github_key - добавить в терминал для vsCode

- ssh -T git@github.com - проверить что есть права

- git push -u origin master - пушим первый комиит
