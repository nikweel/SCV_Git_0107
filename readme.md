
![logo](git-logo.png)
# Работа с Git
## 1. Проверка наличия установленного Git
В терменале выполнить команду `git version` Если git установлен, появится сообщение с информацией о ветрсии программы. Иначе будет сообщение об ошибке.

## 2. Установка Git
Загружаем последнюю версию git с официального сайта:

https://git-scm.com/downloads

Устанавливаем с настройками по умолчанию.

## 3. Настройка Git
При первом использовании git необходимо представиться, для этого вводим две команды в терминале.

```
git config --global user.name "Имя"
git config --global user.email "Эл. почта"
```

## 4. Создание локального репозитория (init / copy)
Создать репозиторий можно двумя способами:
1. Сделать инициализацию командой
```
git init
```
2. Скопировать репозиторий в текущую папку
```
git copy "url"
```
Каждый файл в рабочей папке (репозитории) может быить в одном из двух состояний: под версионным контролем (tracked) и нет (untracked)

## 5. Посмотреть статус текущего репозитория (status)

1. Показать ветку и изменения и вообще папка репозиторий или нет
```
git status
```
2. Сокращенный вывод покажет файлы где были изменения или которые были добавлены
```
git status -s
```

## 6. Добавить файл в отслеживание (add)
1. Добавить определенный файл (xxx)
```
git add xxx
```

2. Добавить все файлы репозитория к отслеживанию
```
git add .
```


## 7. Фиксация изменений (commit)
1. Зафиксировать текуцщие состояние
```
git commit -m "Комментарий к комиту"
```

2. Добавить файлы (измененные) к отслеживанию и зафиксировать текуцщие состояние
```
git commit -a -m "Комментарий к комиту"
```
или
```
git commit -am "Комментарий к комиту"
```
3. Исправить комментарий посдеднего комита
```
git commit -amend -m "Комментарий к комиту исправленный"
```
 
## 8. Получение лога изменений (log)
1. Вывод лога изменений
```
git log
```
*commit xxxxxxxx - id комита*

2. Показать один посдедний коммит
```
git log -1
```
*-2 два последних, -3 три посдедних*

3. Вывод лога изменений + что было изменено
```
git log -p
```
4. Удобный кртаткий лог (id комита - комментарий)
```
git log --oneline
```

5. Лог коммитов (с визуализацией)
```
git log --graph
```
## 9. Переход между коммитами (checkout)

1. Перейти в определенный коммит (xxxx - id коммита)
```
git checkout xxxx
```
2. Перейти в ветку branch_name (на последний коммит ветки branch_name)
```
git checkout branch_name
```

## 10. Показать изменения с последнего коммита (diff)

1. Покажет измеения между текущим и уже закомиченной версией
```
git diff
```

## 11. Работа с ветками (branch)

1. Показать доступные ветки
```
git branch
```
2. Создать новую ветку
```
git branch branch_name
```
3. Удалить ветку (После merge)
```
git branch -d branch_name
```
4. Удалить ветку (Принудительно)
```
git branch -D branch_name
```

## 12. Слияние веток

1. Слить ветки можно командой (в текущую ветку добавит информацию из ветки branch_name)
```
git merge branch_name
```

## 13. Справка о команде

1. Справка о команде xxx
```
git xxx -h
```

## Удаленная работа с GIT
1. Делаем форк проекта если работаем с чужим репозиторием в git вкладка fork
2. Клонируем репозитоорий себе на компьютер через clone или привязываем локальный репозиторий через git remote add origin https://url_git_rep
3. Создаем новую ветку
4. Вносим изменения, коммитим
5. Делаем git push отправляем изменения на удаленный репозиторий
6. В гите делаем pull requvest предлогаем изменения втору репозитория


## Полезный ресурс
Можно эксперементировать с git на данном ресурсе, наверное он так же приносит пользу в обучении
```
https://learngitbranching.js.org/?locale=ru_RU
```

## Обо мне
Работал в школе еникейшщиком, теперь на фрилансе, хочу получить навыки программирования и разработки в целом.

