---
## Front matter
title: "Лабораторная работа № 4"
subtitle: "Отчет"
author: "Казначеев Сергей Ильич"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Получение навыков правильной работы с репозиториями git.

# Задание

Выполнить работу для тестового репозитория.
Преобразовать рабочий репозиторий в репозиторий с git-flow и conventional commits.

# Теоретическое введение

Здесь описываются теоретические аспекты, связанные с выполнением работы.

Например, в табл. [-@tbl:std-dir] приведено краткое описание стандартных каталогов Unix.

: Описание некоторых каталогов файловой системы GNU Linux {#tbl:std-dir}

| Имя каталога | Описание каталога                                                                                                          |
|--------------|----------------------------------------------------------------------------------------------------------------------------|
| `/`          | Корневая директория, содержащая всю файловую                                                                               |
| `/bin `      | Основные системные утилиты, необходимые как в однопользовательском режиме, так и при обычной работе всем пользователям     |
| `/etc`       | Общесистемные конфигурационные файлы и файлы конфигурации установленных программ                                           |
| `/home`      | Содержит домашние директории пользователей, которые, в свою очередь, содержат персональные настройки и данные пользователя |
| `/media`     | Точки монтирования для сменных носителей                                                                                   |
| `/root`      | Домашняя директория пользователя  `root`                                                                                   |
| `/tmp`       | Временные файлы                                                                                                            |
| `/usr`       | Вторичная иерархия для данных пользователя                                                                                 |

Более подробно про Unix см. в [@tanenbaum_book_modern-os_ru; @robbins_book_bash_en; @zarrelli_book_mastering-bash_en; @newham_book_learning-bash_en].

# Выполнение лабораторной работы

Для начала подключим репозиторий из которого можно скачать gitflow

![sc1](image/1.jpg)

После установим gitflow

![sc2](image/2.jpg)

Теперь установим Nodejs

![sc3](image/3.jpg)

Установим pnpm

![sc4](image/4.jpg)

Запустим pnpm

![sc5](image/5.jpg)

Теперь установим с помощью него Commitizien

![sc6](image/6.jpg)

Создаем тестовый репозиторий git-extended

![sc7](image/7.jpg)

И клонируем его себе на компьютер 

![sc8](image/8.jpg)

Создадим какой нибудь файл и проиндексируем его с помощью git add сделав при этом commit

![sc9](image/9.jpg)

Теперь добавим ветку 

![sc10](image/10.jpg)

Теперь обратно запушим на github

![sc11](image/11.jpg)

Теперь проинициализируем pnpm

![sc12](image/12.jpg)

После инициальзации создается файл packege.json который меняем следующим образом 

![sc13](image/13.jpg)

Делаем коммит с помощью cz

![sc14](image/14.jpg)

Проинициализируем gitflow. Укажем название веток и префикс для версий 

![sc15](image/15.jpg)

Выведем список веток и убедимся, что мы находимся в develop, и запушим изменения на сервер 

![sc16](image/16.jpg)

Переключимся на ветку develop после чего создадим ветку релиза где создадим changelog

![sc17](image/17.jpg)

![sc18](image/18.jpg)

Проиндексируем changelog и сделаем коммит 

![sc19](image/19.jpg)

Теперь сольем ветку relaese с веткой changelog

![sc21](image/21.jpg)

Загружаем данные на github

![sc22](image/22.jpg)

Создаем релиз из changelog'a

![sc23](image/23.jpg)

Создаем ветку feature и сразу сливаем ее с develop

![sc24](image/24.jpg)

Создаем ветку релиза

![sc25](image/25.jpg)

Меняем версию в packege.json

![sc26](image/26.jpg)

Создаем ветку журнал изменений, проиндексируем его и сольем ветку с ним в ветку develop

![sc27](image/27.jpg)

Загрузим изменения на гитхаб и создадим релиз 

![sc28](image/28.jpg)

# Вывод

Я получил правильные навыки работы, с репозиториями git

# Список литературы{.unnumbered}

::: {#refs}
:::
