# Репозиторий для **pull request**
* В своём аккаунте на GitHub создать копию репозитория **"AndreyBulgakov19
/SCV_Git_2110"** с помощью кнопки **"Fork"**.
---
* Клонировать копию репозитория на локальный компьютер.
---
* Создать новую ветку.
---
* Добавить файл с инструкцией в новую ветку.
---
* Дополнить инструкцию разделами по работе с удалёнными репозиториями, pull request.
---
* Зафиксировать изменения (коммиты).
---
* Отправить изменения на GitHub.
---
* На сайте GitHub выполнить **Pull request**.
---
# Инструкция к git

##  Проверить, установлен ли git
В терминале выполнить команду `git version`.

Если git установлен, появится сообщение с информацией о версии программы. Иначе будет сообщение об ошибке

##  Уставновка git
Загрузить последнюю версию git с сайта https://git-scm.com/downloads
Устанавливаем с настройками по умолчанию.

## Настройка git
При первой использовании git необходимо представиться. Для этого нужно ввести две команды:
```
git config -- global user.name ""
git config -- global user.email ""
```
## Инициализация репозитория
Для инициализации вводится команда:
```
git init
```
## Статус
Чтобы узнать статус файла (есть ли изменения) используется команда:
```
git status
```
## Отслеживание 
Для отслеживания и подготовки файла к коммиту используется команда:
```
git add <name_file>
```
## Коммит
Для сохранения (фиксации) файла вводитсся команда:
```
git commit -m "комментарий к сохранению"
```
## Исправление комментария
Исправить комментарий в последнем коммите можно с помощью команды:
```
git commit --amend -am "Добавить исправления в комментарий"
```
## Журнал изменений
Для просмотра созданных коммитов (изменений) используется команда:
```
git log
```
## Переход между версиями
Для перехода между версиями вводится команда:
```
git checkout <*>
```
где * - это номер коммита, к которому необходимо перейти

## Сравнение версий
Для того, чтобы сравнить версию с предыдущей вводится команда:
 ```
git diff
```
## Добавление изображений
В квадратных скобках пишется текст, который будет высвечиваться, если изображение не загрузится
Для добавления изображения используется команда:
```
![text](name_image)
```
![Привет](Leo.jpg)

## Игнорирование
Для того, чтобы Git игнорировал файлы, создаем папку `.gitignore`. В эту папку помещаются все файлы, которые необходимо игнорировать:

1. Открываем папку
2. Записываем туда название файла, который надо игнорировать
3. Фиксируем изменения 

## Создание новой ветки
Для создания новой ветки вводится команда:
```
git branch <name_branch>
```

## Просмотр веток
Чтобы вывести список локальных веток используется команда: 
```
git branch
```

## Переход между ветками
Чтобы перемещаться между ветками используется команда: 
```
git branch <name_branch>
```

## Разрешение конфликтов
Чтобы разрешить конфликт слияния, вызванный конкурирующими изменениями строк, нужно выбрать, какие изменения из разных ветвей включить в новую фиксацию. Для этого при появлении в терминале сообщения о конфликте, VSC предложит сохранить версию текущей ветки, сохранить версию вливаемой ветки или сохранить сразу обе, после чего можно будет отредактировать конечную версию вручную.


## Удаление веток

Чтобы удалить ненужную ветку, необходимо набрать команду:
```
git branch -d <name_branch>
```

## Слияние
Для слияния двух веток набирается команда:
```
git merge <name_branch>
```

## Работа с удаленными репозиториями
  1. Клонировать удаленный репозиторий:
  ```
  git clone <адрес удаленного репозитория>
  ```
  2. Добавить изменения в удаленный репозторий
  ```
  git push 
  ```
    
**Важно! Для обмена между локальным и удаленным репозиториями названия веток должны быть одинаковыми.**
   
 3. Загрузить изменения из удаленного репозитория:
    ```
    git pull
    или    
    git fetch
    ```
   4. Проверить, связаны ли удаленный и локальный репозитории (появятся 2 адреса):
   ```
   git remote -v 
   ```
  5. **Pull request** - запрос на добавление изменений в проект.
  Для этого необходимо скопировать репозиторий с помощью кнопки `Fork` в свой аккаунт. Все последующие изменения и добавления выполняются в склонированном репозитории и загружаются в удаленный репозиторий. После этого в удаженном  репозитории появится кнопка  **Pull request**.


## Заключение

Будучи контентно-адресуемой файловой системой, Git является мощным инструментом, который может применяться не только как VCS. 
