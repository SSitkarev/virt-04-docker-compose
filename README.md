# Домашнее задание к занятию 4. «Оркестрация группой Docker-контейнеров на примере Docker Compose» - Ситкарёв Сергей

## Задача 1

Создайте собственный образ любой операционной системы (например ubuntu-20.04) с помощью Packer (инструкция).

Чтобы получить зачёт, вам нужно предоставить скриншот страницы с созданным образом из личного кабинета YandexCloud.

Данное задание выполнить невозможно.

Самая свежая версия packer 1.9.1 не работает с яндексом - error initializing builder 'yandex': Unknown builder yandex

Установил версию 1.5.0

Сначала получил токен https://oauth.yandex.ru/authorize?response_type=token&client_id=блабла

Инициализировал yc дважды, всё успешно.

![Задание1](https://github.com/SSitkarev/virt-04-docker-compose/blob/main/img/1_1.png)

packer конфиг файл 

![Задание1](https://github.com/SSitkarev/virt-04-docker-compose/blob/main/img/1_2.png)

Везде использую один и тот же токен, однако получаю ошибку при сборке имиджа

![Задание1](https://github.com/SSitkarev/virt-04-docker-compose/blob/main/img/1_3.png)

## Задача 2

Создайте вашу первую виртуальную машину в YandexCloud с помощью web-интерфейса YandexCloud.

![Задание2](https://github.com/SSitkarev/virt-04-docker-compose/blob/main/img/2.png)

## Задача 3

С помощью Ansible и Docker Compose разверните на виртуальной машине из предыдущего задания систему мониторинга на основе Prometheus/Grafana. Используйте Ansible-код в директории (src/ansible).

Чтобы получить зачёт, вам нужно предоставить вывод команды "docker ps" , все контейнеры, описанные в docker-compose, должны быть в статусе "Up".

![Задание3](https://github.com/SSitkarev/virt-04-docker-compose/blob/main/img/3.png)

## Задача 4

Откройте веб-браузер, зайдите на страницу http://<внешний_ip_адрес_вашей_ВМ>:3000.
Используйте для авторизации логин и пароль из .env-file.
Изучите доступный интерфейс, найдите в интерфейсе автоматически созданные docker-compose-панели с графиками(dashboards).
Подождите 5-10 минут, чтобы система мониторинга успела накопить данные.
Чтобы получить зачёт, предоставьте:

скриншот работающего веб-интерфейса Grafana с текущими метриками, как на примере ниже.

![Задание3](https://github.com/SSitkarev/virt-04-docker-compose/blob/main/img/4.png)