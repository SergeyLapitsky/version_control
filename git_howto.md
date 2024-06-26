# Подсказка по GIT

## Создание репозитория:
```sh
git init
```
## Выбор файла для сохранения
```sh
git add <filename>
```

## Фиксирование изменений в файле
```sh
git commit -m "Message text"
```
## Просмотр сохраненных версий файла
```sh
git log
```
### В сокращенном виде:
```sh
git log --oneline
```
## Переход между версиями файла
```sh
git checkout <первые 4 символа коммита>
```
## Переход между ветками 
```sh
git checkout <имя_ветки>
```

## Отображение всех веток
```sh
git branch
```
## Создание новой ветки
```sh
git branch <имя_ветки>
```
## Слияние веток
**Выполнять из ветки master!**
```sh
git merge <имя_ветки>
```
## Удаление ветки
```sh
git branch -d <имя_ветки>
```
## Графическое отображение веток и коммитов
В обычном виде:
```sh
git log --graph
```
В сокращенном виде:
```sh
git log --oneline --graph
```

## Просмотр удалённых репозиториев
Для того, чтобы просмотреть список настроенных удалённых репозиториев, вы можете запустить команду
```sh
git remote
```
Вы можете также указать ключ -v, чтобы просмотреть адреса для чтения и записи, привязанные к репозиторию:
```sh 
origin	https://github.com/... (fetch)
origin	https://github.com/... (push)
```
## Добавление удалённых репозиториев
Для того, чтобы добавить удалённый репозиторий и присвоить ему имя (shortname), просто выполните команду:
```sh
git remote add <shortname> <url>
```
## Отправка изменений в удалённый репозиторий (Push)
Когда вы хотите поделиться своими наработками, вам необходимо отправить их в удалённый репозиторий. Команда для этого действия: 
```sh
git push <remote-name> <branch-name>
``` 
Чтобы отправить вашу ветку master на сервер origin, вы можете выполнить следующую команду для отправки ваших коммитов:
```sh
git push origin master
```
## Просмотр удалённого репозитория
Если хотите получить побольше информации об одном из удалённых репозиториев, вы можете использовать команду:
```sh
git remote show <remote>
```
Например:
```sh
git remote show origin
``` 