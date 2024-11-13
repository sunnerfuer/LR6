# Лабораторная работа №6

## Система контроля версий
**Введение**

**Цель работы**

Изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.

**Задание**

1. Создать аккаунт на сайте GitHub;
2. Сделать копию в личное хранилище из https://github.com/Kurtyanik/LR6/ (Fork);
3. Установить Git;
4. Настроить клиент git, введя имя пользователя (Группа Фамилия И.О.) и email;
5. Клонировать свой личный удалённый репозиторий на компьютер;
6. Добавить файл через интерфейс GitHub. Подтянуть изменения в локальный репозиторий;
7. Получить историю операций для каждой из веток;
8. Посмотреть последние изменения;
9. Выполнить слияние в ветку master, разрешив конфликт;
10. Удалить побочную ветку после успешного слияния;
11. Сделать изменения и зафиксировать их, оставляя комментарии, несколько раз;
12. Сделать откат коммита;
13. Создать ветку для отчёта;
14. Начать оформлять отчёт в файле README.md, используя markdown синтаксис;
    - В отчёте должен быть снимки экрана консоли и сторонних программ. Файлы снимков экрана разместить в отдельной папке.
    - Лог команд (без результатов их выполнения).
15. Получить историю операций в форматированном виде (сокращённый хэш + дата + имя автора + комментарий);
16. Отправить локальные изменения в сетевое хранилище GitHub.

**Ход выполнение**

Аккаунт на GitHub был создан некоторое время назад, поэтому
готовый аккаунт представлен на рисунке 1.

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/profile.jpg">
</p>
<p align="center">Рисунок 1 - Профиль в Git Hub</p></br>

Следующим этапом стало создание форка репозитория (https://github.com/Kurtyanik/LR6/ ). Таким образом, была создана копия данного репозитория в моём личном профиле. Скриншот созданной копии представлен на рисунке 2.

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/fork.jpg">
</p>
<p align="center">Рисунок 2 - Готовый fork репозитория</p></br>

> [!IMPORTANT]
> При создании форка необходимо убрать галочку перед согласием копирования исключительно ветки master
>
Следующим шагом было необходимо установить Git, однако он уже был установлен. Поэтому далее происходила настройка клиента git, где было необходимо ввести имя пользователя и почту (рисунок 3-4). В ходе данной процедуры будут произведены следующие глобальные изменения:

- установленное имя будет использоваться в качестве автора коммита
- установленная электронная почта будет связывать коммиты с конкретным пользователем

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/user_name%20and%20email.jpg">
</p>
<p align="center">Рисунок 3 - Настройка клиента git</p></br>

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/git%20config.jpg">
</p>
<p align="center">Рисунок 4 - Результаты настройки клиента git</p></br>

Далее было необходимо клонировать репозиторий с сервера на личный компьютер (рисунок 5).

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/cloning.jpg">
</p>
<p align="center">Рисунок 5 - Клонирование репозитория</p></br>

Файл добавлялся через интерфейс Git Hub в главную ветку репозитория (рисунок 6).

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/adding%20file.jpg">
</p>
<p align="center">Рисунок 6 - Добавление файла</p></br>

Данное действие удобно для создания новых файлов или небольших правок. Но для более сложных задач чаще используют локальную среду и, так как по заданию необходимо производить редактирование веток и решение конфликтов, остальные задачи будут производиться локально в среде Git. Для этого было проведено обновление рабочей копии репозитория, путём подтягивания последних изменеий из удалённого репозитория. Далее была произведена операция просмотра историй операций на каждой ветке (рисунок 7-8)

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/git%20log%20master!.jpg">
</p>
<p align="center">Рисунок 7 - История операций ветки master</p></br>

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/git%20log%20branch1.jpg">
</p>
<p align="center">Рисунок 8 - История операций ветки branch1</p></br>

> [!TIP]
> Для правильного выполнения пункта необходимо сначала перейти в желаемую ветку через команду `cd`.

> [!NOTE]
> Также можно посмотреть [историю двух веток](https://github.com/sunnerfuer/LR6/blob/report/screenshots/showing%20hostory%20of%202.jpg) при помощи команды `gitk --all`.

 Для просмотра последних изменений в ветках использовалась команда `git show` (рисунок 9-10). Таким образом, можно наблюдать основную информацию о коммите (хэш, автора, дату создания, содержание и внесённые изменения)

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/git%20show%20master.jpg">
</p>
<p align="center">Рисунок 9 - Последние изменения в ветке master</p></br>

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/git%20show%20branch1.jpg">
</p>
<p align="center">Рисунок 10 - Последние изменения в ветке branch1</p></br>

Далее было необходимо произвести слияние в ветку master, данный шаг представлен на рисунке 11.

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/git%20checkout%20master.jpg">
</p>
<p align="center">Рисунок 11 - Слияние в ветку master</p></br>

> [!WARNING]
> При попытке слияния двух файлов с одинаковым названием, но разным содержимым, произойдет конфликт. Для разрешения конфликта необходимо применить команду `notepad mergefile.txt` и внести изменения в конфликтующем содержимом (рисунок 12-13)

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/merge1.jpg">
</p>
<p align="center">Рисунок 12 - Конфликтующий файл</p></br>

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/merge2.jpg">
</p>
<p align="center">Рисунок 13 - Решение конфликта</p></br>

После произведенных манипуляций необходимо добавить измененный файл с помощью команды `git add mergefile.txt`. Результат представлен на рисунке 14.

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/git%20add%20merge.jpg">
</p>
<p align="center">Рисунок 14 - Добавление измененного файла</p></br>

После успешного слияния необходимо удалить ветку branch1 (рисунок 15).

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/git%20branch%20delete.jpg">
</p>
<p align="center">Рисунок 15 - Удаление ветки branch1</p></br>

Для создания нескольких изменений использовалась команда `echo`, с помощью которой было создано два файла (рисунок 16-17).

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/echo%201.jpg">
</p>
<p align="center">Рисунок 16 - Создание первого файла changes</p></br>

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/echo2.jpg">
</p>
<p align="center">Рисунок 17 - Создание второго файла changes2</p></br>

> [!NOTE]
> Для просмотра содержимого файлов удобно использовать команду `cat`

Следующим этапом было необходимо произвести откат коммита. Данный шаг можно наблюдать на рисунке 18.

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/git%20reset.jpg">
</p>
<p align="center">Рисунок 18 - Откат коммита</p></br>

> [!NOTE]
> Флаг `-3` отображает последние 3 коммита в текущей ветке репозитория

Для создания и оформления отчета была создана отдельная ветка (рисунок 19).

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/git%20branch%20report.jpg">
</p>
<p align="center">Рисунок 19 - Создания ветки для отчета</p></br>

Последним этапом было необходимо выполнить получение истории операций в форматированном виде (сокращённый хэш + дата + имя автора + комментарий), что представлено на рисунке 20.

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/format.jpg">
</p>
<p align="center">Рисунок 20 - История операций в форматированном виде</p></br>

**Лог команд**
```
git config --global user.name "4315 Deryabina Mary Alexeevna"
git config --global user.email "deryabina.masha.2005@gmail.com"
git config --global --list 
git clone https://github.com/sunnerfuer/LR6
cd LR6
git pull 
git log master
git log branch1
gitk --all
git show master
git show branch1  
git checkout master
git merge branch1
git status
notepad mergefile.txt
git add mergefile.txt
notepad mergefile.txt
git add mergefile.txt
git status
git commit -m "Branches successfully connected (conflict resolved)"
git branch -d branch1
git branch   
echo "Was created the first note" >> changes.txt 
git add changes.txt  
cat changes.txt
git status
git commit -m "Was created the second note"
echo "Was created the second note" >> changes2.txt 
git add changes2.txt  
cat changes2.txt
git status
git commit -m "Was created the second note"
git reset HEAD~1
git log -3
git branch report
git branch
git push
git push origin report
git log --date=format:'%D' --pretty=format:"%h -> %cd, %cn ( %s )"
history
```

**Выводы**

В ходе лабораторной работы был изучен Git, а также получен опыт работы с GitHub и Git API. 
В процесе выполнения работы был получен практический опыт работы с репозиторием, средой git, с ветками, разрешением их конфликтов, созданием файлов. Был изучен формат Markdown для оформления отчета.

