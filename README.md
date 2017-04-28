<p align="center">
  <img src='misc/pereval_logo.png'/>
</p>

# The Pereval server

_In develompent_

## Описание

**Перевал** - это сборка настроенных open-source web-сервисов, которую можно установить на локальной виртуальной машине или на удалённом сервере. Сервисы предназначены для совместной деятельности небольших групп людей. В качестве точки входа выступает дашбоард на главной странице сервиса, в котором предоставляется системная информация и данные по каждому из сервисов.

Проект является аналогом широко известного [TurnKey](https://www.turnkeylinux.org/), позволяющего скачать и развернуть на любой платформе одну из готовый сборок специализированных серверов c предустановленным программным обеспечением.

_Предназначение_: индивидуальная либо совместная работа над деятельностью по поиску, сбору, и хранению информации (OSINT), а также сопутствующая коммуникация. 

_Области применения_: пентестинг (подготовка к тестированию на проникновение), конкурентная разведка (сбор информации по людям, доменам, аккаунтам), нетсталкинг (поиск, анализ и архивирование различной информации).

_Мотивация_: часто разнообразная деятельность, связанная с поиском, агрегацией и анализом информации упирается в недостаточность квалификации человека и отсутствие удобных инструментов для автоматизации деятельности. Сконфигурированные сборки web-сервисов, устанавливающиеся в несколько кликов, позволят ускорить работу и повысить её эффективность, а также распределить задачи между людьми.

Черновик описания проекта смотреть [здесь](https://hackpad.com/ep/pad/static/EoF3ngu7pXM).

## Запуск

1. Установить Docker и Docker Compose
1. Склонировать репозиторий и развернуть сервер:
```
git clone https://github.com/pereval-team/pereval-server.git
cd pereval-server && sudo docker-compose up --build
```

## Сервисы

<p align="center">
  <img src='https://hackpad-attachments.s3.amazonaws.com/hackpad.com_EoF3ngu7pXM_p.724442_1491844991468_undefined'/>
</p>


- [OSINT](#OSINT)

  - [Анализ](#Анализ)

  - [Поиск](#Поиск)

- [Записи](#Записи)

  - [Базы знаний](#Базы_знаний)
  
  - [Текст](#Текст)

  - [Таблицы](#Таблицы)

  - [Схемы](#Схемы)

- [Архивирование](#Архивирование)

  - [Файлы](#Файлы)
  
  - [Ссылки](#Ссылки)

  - [Веб-контент](#Веб-контент)

- [Централизация](#Централизация)

- [Коллаборация](#Коллаборация)

### OSINT

К сервисам для OSINT (Open source intelligence, разведка на основе открытых источников) отнесены веб-приложения, позволяющие искать информацию через API других сервисов, путём сканирования URL и IP, а также веб-приложения для анализа данных.

#### Поиск

- IVRE

- Spiderfoot

- Intrigue

- Openwebspider

#### Анализ

- CyberChef

### Записи

#### Базы знаний

- dokuwiki

- XWiki

- PmWiki

#### Текст 

- Hackerpad

- Paperwork

- CryptPad

- Etherpad

#### Таблицы

- EtherCalc

- Ethersheets

#### Схемы

- Wisemapping

### Архивирование

#### Файлы

- Nextcloud

- Webrecorder

#### Ссылки

- wallabag

#### Веб-контент

- Bookmarks

### Централизация

- pereval-dash

- OpenLDAP - для защиты доступа в большое количество сервисов так или иначе требуется единый реестр учётных записей. Опциональным средством в рамках Перевала может быть авторизация через LDAP, настраиваемая с помощью специального софта.

### Коллаборация

#### Средства общения

- converse.js

- KiwiIRC

#### Ведение задач

- Wekan

- Taskboard

- Kanboard

- Restya
