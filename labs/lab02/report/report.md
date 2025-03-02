---
## Front matter
title: "Первоначальна настройка git"
subtitle: "Лабораторная работа №2"
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

Изучить идеологию и применение средств контроля версий.
Освоить умения по работе с git.

# Задание

Создать базовую конфигурацию для работы с git.
Создать ключ SSH.Создать ключ PGP.
Настроить подписи git.
Зарегистрироваться на Github.
Создать локальный каталог для выполнения заданий по предмету.

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
Для начала установим Git

![sc1](./image/screen1.jpg)

Теперь установим gh 

![screen2](./image/screen2.jpg)

Далее задаем имя владельца репозитория

![sc3](./image/screen3.jpg)

Далее задаем почту владельца git 

![sc_3](./image/screen3.jpg)

Далее настроим котировку UTF-8 в выводе сообщения git 

![sc_3_1](./image/screen3.jpg)

Зададим имя начальной ветки настроим параметры autocrlf и safecrlf

![sc4](./image/screen4.jpg)

Создадим ключ RSA размером 4096 бит

![sc5](./image/screen5.jpg)

Теперь создаем ключ по алгоритму ed22519 

![sc6](./image/screen6.jpg)

Теперь создаем gpg, выбираем из предложенных вариантов первый тим(тип RSA and RSA),размер 4096 бит  и делаем срок ключа неограниченным

![sc7](./image/screen7.jpg)

После нас просят ввести свои данные. Мы вводим имя и адрес электронной почты. После этого соглашаемся с генерацией ключа 

![sc8](./image/screen8.jpg)

Далее выводим список ключей gpg

![sc9](./image/screen9.jpg)

Копируем наш ключ в буфер обмена

![sc10](./image/screen10.jpg)

Вставляем ключ на Github и задаем ему имя

![sc11](./image/screen11.jpg)

Теперь произведем автоматическую настройку подписей
![sc12](./image/screen12.jpg)
	

После нам нужно авторизироватся в  github с помощью gh. Мы выбираем сайт для авторизации(Github),после выбираем 
предпочитаемый протокол (SSH), публичный ключ SSH ключ (id_rsa.pub) и имя для ключа sway. В качестве способа авторизации выбираем авторизацию через браузер 

![sc13](./image/screen13.jpg)

Теперь создаем рабочую директорию курса и переходим в неё

![sc14](./image/screen14.jpg)

Создаем репозиторий для лабораторных работ из шаблона 

![sc15](./image/screen15.jpg)

И клонируем его к себе на компьютер 

![sc16](./image/screen16.jpg)


Переходим в него с помощью cd и удаляем файл(package.json) и создаем необходимые каталоги записав в файл COURSE
строку echo os-intro и прописываем make prepare для того, чтобы нужные нам каталоги создались

![sc17](./image/screen17.jpg)

Теперь добавляем нашу папку для отправки 

![sc18](./image/screen18.jpg)

Делаем коммит в котором указываем что мы сделали структуру курса
		
![sc19](./image/screen19.jpg)

И отправляем файлы на Github с помощью команды push 

![sc20](./image/screen20.jpg) 

# Выводы

Я изучил идеологию и применение средств контроля версий и освоил умения по работе с git 

# Список литературы{.unnumbered}

::: {#refs}
:::
