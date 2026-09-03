# Домашнее задание к занятию «Работа с roles»
Выполнил: Береснев Игорь Андреевич

---

Ваша цель — разбить ваш playbook на отдельные roles.

Задача — сделать roles для ClickHouse, Vector и LightHouse и написать playbook для использования этих ролей.

Ожидаемый результат — существуют три ваших репозитория: два с roles и один с playbook.

Что нужно сделать

    Создайте в старой версии playbook файл requirements.yml и заполните его содержимым:

    ---
      - src: git@github.com:AlexeySetevoi/ansible-clickhouse.git
        scm: git
        version: "1.13"
        name: clickhouse 

При помощи ansible-galaxy скачайте себе эту роль.

Создайте новый каталог с ролью при помощи ansible-galaxy role init vector-role.

На основе tasks из старого playbook заполните новую role. Разнесите переменные между vars и default.

Перенести нужные шаблоны конфигов в templates.

Опишите в README.md обе роли и их параметры. Пример качественной документации ansible role по ссылке.

Повторите шаги 3–6 для LightHouse. Помните, что одна роль должна настраивать один продукт.

Выложите все roles в репозитории. Проставьте теги, используя семантическую нумерацию. Добавьте roles в requirements.yml в playbook.

Переработайте playbook на использование roles. Не забудьте про зависимости LightHouse и возможности совмещения roles с tasks.

Выложите playbook в репозиторий.

В ответе дайте ссылки на оба репозитория с roles и одну ссылку на репозиторий с playbook.

1. Задача

Разбить плейбук на роли для ClickHouse, Vector и LightHouse. Создать три репозитория: два с ролями и один с плейбуком.

2. Выполненные действия

    Создан файл requirements.yml со ссылками на роли.

    Скачана роль ClickHouse из внешнего репозитория.

    Созданы роли Vector и Lighthouse.

    В каждой роли заполнены все необходимые файлы.

    Написан плейбук site.yml с использованием всех ролей.

    Создан inventory.ini для хостов.

    Роли выложены в отдельные репозитории с тегами v1.0.0.

    Плейбук выложен в отдельный репозиторий.

3. Репозитории

https://github.com/BeresnevIA/Vector

https://github.com/BeresnevIA/Lighthouse

https://github.com/BeresnevIA/Playbook
