---
## Front matter
title: "Лабораторная работа №5"
subtitle: "Отчет"
author: "Казанчеев Сергей Ильич"

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

Научится пользоватся pass и chezmoi

# Задание

Настроить OC  синхронизируя ее с данной
Научится использовать программы для управления паролями


# Выполнение лабораторной работы

Для начала необходимо установить pass и pass-out

![1](image/1.png)

Установим gopass

![2](image/2.png)

Выведем список pgp  ключей

![3](image/3.png)

Проинициализируем pass, указав свой email

![4](image/4.png)

Проинициализируем репозиторий с git  для pass

![5](image/5.png)

Создадим репозиторий pass

![6](image/6.png)

Пробуем получить данные 

![7](image/7.png)

Но не получаем так как репозиторий пуст. Выложим изменения на Github

![8](image/8.png)

Теперь снова пробуем получить данные 

![9](image/9.png)

Сделаем пустой коммит и выложим его 

![10](image/10.png)

Проверим статус pass репозитория 

![11](image/11.png)

Подключим репозиторий для скачивания browserpass

![12](image/12.png)

установим browserpass

![13](image/13.png)

и установим его в браузере 

![14](image/14.png)

Создадим файл с паролем 

![15](image/15.png)

И установим дополнительные пакеты 

![16](image/16.png)

Подключим репозиторий для скачивания шрифтов 

![17](image/17.png)
 
Найдем шрифты 

![18](image/18.png)

И установим

![19](image/19.png)

Установка chezmoi

![20](image/20.png)

Создадим репозиторий из шаблона

![21](image/21.png)

Проинициализируем chezmoi, указав только что созданные репозиторий

![22](image/22.png)

Посмотрим на изменения 

![23](image/23.png)

И согласимся с ними

![24](image/24.png)

Проинициализируем chezmoi на второй машине 

![25](image/25.png)

Посмотрим изменения 

![26](image/26.png)

И согласимся с ними 

![27](image/27.png)

Извлечем изменения из репозитория 

![28](image/28.png)

И отредактируем конфигурационный файл чтобы автоматически фиксировать изменения в исходный каталог в репозиторий 

![29](image/29.png)

# Выводы

В результате я научился пользоватся pass и chezmoi

