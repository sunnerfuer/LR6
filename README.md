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
8. Получить историю операций для каждой из веток;
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
Следующим шагом было необходимо установить Git, однако он уже был установлен. Поэтому далее происходила настройка клиента git, где было необходимо ввести имя пользователя и почту (рисунок 3). В ходе данной процедуры будут произведены следующие глобальные изменения:

- установленное имя будет использоваться в качестве автора коммита
- установленная электронная почта будет связывать коммиты с конкретным пользователем

<p align="center">
  <img src="https://github.com/sunnerfuer/LR6/blob/report/screenshots/user_name%20and%20email.jpg">
</p>
<p align="center">Рисунок 3 - Настройка клиента git</p></br>