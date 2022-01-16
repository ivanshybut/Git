# Git

## __Создание репозитория__
Создать новый локальный репозиторий
```git
git init [project name]
```
Скачать с существующего репозитория 
```git
git clone my_url
```
##  __Отслеживание репозитория__
Просмотреть список новых или измененных файлов, которые еще не закомитены
```git
git status
```
Показать изменения в файлах, которые еще не поставленны
```git
git diff
```
Показать изменения в индексированных файлах
```git
git diff --cached
```
Показать различия между двумя коммитами
```git
git diff commitl commit2
```
Показать дату изменения и автора для файла 
```git
git blame [file]
```
Показать изменения для определенного коммита и/или файла
```git
git show [commit] : [file]
```
Показать полную историю изменений
```git
git log
```
Показать историю изменений для файла/папки включая различия
```git
git log -p [file/derectory]
```
## Работа с ветками
Показать все локальные ветки
```git
git branch
```
Показать все локальные и удаленные ветки
```git
git branch -av
```
Переключитьсяк ветке my_branch и обновить рабочую директорию
```git
git checkout my_branch
```
Создание новой ветки с изменением new_branch
```git
git branch new_branch
```
Удалить ветку с именем my_branch
```git
git branch -d my_branch
```
Объединить branch_a в branch_b
```git
git checkout branch_b
git merge branch_a
```
Добавить Tag к текущему коммиту
```git
git tag my_tag
```
## Изменения
Индексировать файл готовый к коммиту
```git
git add [file]
```
Индексировать все файлы готовые к коммиту
```git 
git add .
```
Зафиксировать индексированные файлы с комментарием в историю
```git
git commit -m "commit message"
```
Зафиксировать все отслеживаемые файлы с комментарием
```git
git commit -am "commit message"
```
Неиндексированные файлы, получить изменения файла
```git
git resset [file]
```
Откатить все до последней фиксации
```git
git reset ---hard
```
## Синхронизация
Получить последние изменения с удаленного сервера(без слияния)
```git
git fetch
```
Получить последние изменения с удаленного сервера и слияния
```git
git pull
```
Получить последние изменения с удаленного сервера и перебазировать
```git
git pull --rebase
```
Применить лакальные изменения на удаленный сервер
```git
git push
```
### Финал
## В случае сомнений, используйте помощь
```git
$git command --help
```
