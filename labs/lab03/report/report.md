---
## Front matter
title: "Отчёт по лабораторной работе 3"
subtitle: "Архитектура компьютера"
author: "Балаганова Алтана Владиславовна"

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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
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

Целью работы является освоение процедуры оформления отчетов с помощью легковесного языка разметки Markdown.

# Выполнение лабораторной работы

Установили программы pandoc и TexLive по указаниям в лабораторной работе. 

1. Я запустила терминал.

2. Затем я перешла в папку курса, которую создала во время выполнения второй лабораторной работы, 
и обновила локальный репозиторий, загрузив последние изменения из удаленного репозитория.

3. После этого я открыла папку с шаблоном отчёта для лабораторной работы № 3.

4. Я скомпилировала шаблон, используя Makefile. Для этого мне нужно было ввести команду `make`. 
Если всё прошло успешно, то должны были появиться файлы report.pdf и report.docx, 
которые я открыла, чтобы проверить, что всё правильно сформировалось.

docx создался сразу, для pdf потребовалось загрузить шрифты.

![Make шаблона](image/01.png){ #fig:001 width=70%, height=70% }

![Полученные файлы](image/02.png){ #fig:002 width=70%, height=70% }

5. Затем я удалила эти файлы, опять же используя Makefile, введя команду `make clean`. 
Я убедилась, что после этого действия файлы report.pdf и report.docx были действительно удалены.

![Удалены docx и pdf](image/03.png){ #fig:003 width=70%, height=70% }

6. Потом я открыла файл report.md в текстовом редакторе, например, в gedit, и внимательно изучила его структуру.

![report.md](image/04.png){ #fig:004 width=70%, height=70% }

7. Далее я заполнила отчет и снова скомпилировала его с помощью Makefile, чтобы убедиться, что 
всё отображается корректно. 

![Заполним шаблон для отчета](image/05.png){ #fig:005 width=70%, height=70% }

8. После всех этих шагов я загрузила файлы на Github.

9. В качестве дополнительного задания я создала отчет в формате md для второй лабораторной работы.

![Заполним шаблон для отчета](image/06.png){ #fig:006 width=70%, height=70% }

# Выводы

Изучили синтаксис языка разметки Markdown, получили отчет из шаблона при помощи Makefile. 

