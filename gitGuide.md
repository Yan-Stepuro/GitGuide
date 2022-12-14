# Руководство по работе с git

## Термины и определения

**Контроль версий**, также известный как управление исходным кодом, — это практика отслеживания изменений программного кода и управления ими.

**Системы контроля версий** — это программные инструменты, помогающие командам разработчиков управлять изменениями в исходном коде с течением времени.

**Репозиторий** — это все файлы, находящиеся под контролем версий, вместе с историей их изменения и другой служебной информацией. Репозиторий Git можно создать, либо выбрав любую папку на компьютере, либо клонировав себе уже существующий репозиторий.

**Git** *(читается как «гит»)* — это система контроля версий, которая помогает отслеживать историю изменений в файлах. Git используют программисты для совместной работы над проектами.

## Начало работы с Git

Для начала работы с Git требуется скачать необходимое ПО, запустить и прописать первые команды:

1. Скачать Git с официального сайта https://git-scm.com/ и установить
2. Скачать Visual Studio Code с официального сайта https://code.visualstudio.com/ и установить
3. Запустить Visual Studio Code
4. В терминале прописать команды для начала работы:
    * Задать имя пользователя: **git config --global user.name**
    * Задать почту пользователя: **git config --global user.email**
5. Задать папку для создания репозитория
6. Создать репозиторий при помщи команды **git init**
7. Создать или выбрать файл  

## Команды Git

В Git для работы используются следующие команды: 
* **git config --global _user.name_** - задать имя пользователя
* **git config --global _user.email_** - задать электронную почту пользователя
* **git init** - преобразовать папку в репозиторий
* **git add _имя_файла_** - добавить изменения из рабочего каталога в индекс для последующего коммита
* **git commit** - фиксирует состояние проекта на текущий момент. Данную команду рекомендуется использовать с параметром **-m "_комментарий_"**, который позволяет добавить пояснительный комментарий к коммиту. Итоговая команда будет выглядеть следующим образом: **git commit -m "_комментарий_"**
* **git log** - отображает историю коммитов.
* **git status** - отображает состояние рабочего каталога и раздела проиндексированных файлов. С ее помощью можно проверить индексацию изменений и увидеть файлы, которые не отслеживаются Git.
* **git diff** - показывает изменения в вашей рабочей директории, которые еще не были добавлены в индекс для последующего коммита.
* **git branch _имя ветки_** - создает новую ветку с именем _имя файла_
* **git branch** - отображает существующие ветки. Активная ветка помечается звездочкой (*)
* **git checkout _имя ветки_** - переключает активную ветку на _имя ветки_ . Можно переключаться только между существующими ветками
* **git merge _имя ветки_** - добавляет данные из ветки _имя ветки_ в активну ветку. При добавлении (слиянии) веток происходит анализ данных на соответствие. Если происхоит конфликт, когда в одном и том же месте расположена разная информация, система предложит разрешить конфликт одним из нескольких способов: оставить текущую версию, принять входящую версию, оставить оба варианта. Можно разрешить конфликт и вручную отредактировав документ.

## GitHub

[GitHub](https://github.com/ "Официальный сайт GitHub") — это облачная платформа для хостинга IT-проектов и совместной разработки, в основе которой которой находится популярная система контроля версий Git, а также полноценная социальная сеть для разработчиков. GitHub предоставляет широкий набор инструментов для хранения и шеринга проектов, а так же совместной работы над ними. 

Начало работы с GitHub:
1. Создать аккаунт на сайте github.com
2. Создать новый репозиторий
3. Связать локальный и удаленный репозитории

Команды для работы с github:
* **git clone _ссылка на репозиторий_** - копирует удаленный репозиторий
* **git remote add origin _ссылка на репозиторий_** - связывает локальный и удаленный репощзитории
* **git branch -M main** - указывает, какая ветка будет являться основной
* **git push -u origin** - отправляет репозиторий с локального хранилища в удаленное 
* **git push** - отправляет изменения из локального репозитория в связанный с ним удаленный репозиторий
* **git pull** - забирает репозиторий с удаленного хранилища в локальное и сливает их (merge)
