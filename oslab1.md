---
# Front matter
title: "Лабораторная работа 1"
subtitle: "Отчёт"
author: "Новосельцев Данила Сергеевич"

# Generic otions
lang: ru-RU
toc-title: "Содержание"

# Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

# Pdf output format
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
### Fonts
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
## Misc options
indent: true
header-includes:
  - \linepenalty=10 
  - \interlinepenalty=0 
  - \hyphenpenalty=50 
  - \exhyphenpenalty=50 
  - \binoppenalty=700 
  - \relpenalty=500 
  - \clubpenalty=150 
  - \widowpenalty=150 
  - \displaywidowpenalty=50 
  - \brokenpenalty=100 
  - \predisplaypenalty=10000 
  - \postdisplaypenalty=0 
  - \floatingpenalty = 20000 
  - \raggedbottom 
  - \usepackage{float} 
  - \floatplacement{figure}{H} 
---

# Лабораторная работа 5
 Новосельцев.Д.С. 
 НФИбд-02-20

---


Цель работы: приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для
дальнейшей работы сервисов.

---

Ход работы:

Загрузил Virtualbox на свой компьютер.

Создал новую виртуальную машину. Указал имя виртуальной машины, тип операционной системы — Linux, Ubuntu.
![Linux](https://imgur.com/tHW3Kic.png)
![memory](https://imgur.com/8cZBLAy.png)
![disk](https://imgur.com/UlorMbu.png)
![type](https://imgur.com/WcTewqQ.png)
![format](https://imgur.com/0l4lYPa.png)
![name](https://imgur.com/Tv1Gg5t.png)
![CentOS](https://imgur.com/Rggun5s.png)
![test](https://imgur.com/SzSIyAl.png)
![time](https://imgur.com/aZzS9Z0.png)
![tools](https://imgur.com/17LPymF.png)
![kdump](https://imgur.com/2NESCWM.png)
![host](https://imgur.com/eNZGgbo.png)
![Ethernet](https://imgur.com/ECCbErx.png)
![password](https://imgur.com/UYPMmRX.png)
![User](https://imgur.com/qTvME7f.png)

Дождался загрузки графического окружения и открыл терминал.

С помощь команды dmesg | grep -i «то, что я ищу» получил следующую информацию:

1. Версия ядра Linux (Linux version).
![Linux version](https://imgur.com/DF5Xiwh.png)
2. Частота процессора (Detected Mhz version).
![Detected Mhz version](https://imgur.com/k1bbhOj.png)
3. Модель процессора (CPU0).
![CPU0](https://imgur.com/1M9yz9f.png)
4. Объём доступной оперативной памяти (Memory available).
![Memory available](https://imgur.com/hojymC0.png)
5. Тип обнаруженного гипервизора (Hypervisor detected).
![Hypervisor detected](https://imgur.com/nMjmbEN.png)
6. Тип файловой системы корневого раздела.
![filesystem](https://imgur.com/vgVjbJl.png)
7. Последовательность монтирования файловых систем.
![mount](https://imgur.com/A1OJrOI.png)

Вывод: приобрёл практические навыки установки операционной системы на виртуальную машину, настройки минимально необходимых для
дальнейшей работы сервисов.

Ответы на контрольные вопросы:

1. Учётная запись содержит данные о пользователе, необходимые для регистрации в системе и дальнейшей работы с ней.

2. - Команда man используется для получения справки о любой команде системы. Например, команда man is выведет справку об использовании команды is, которая выводит содержимое каталога.

- Для перемещения по файловой системе используется команда cd. Например, чтобы перейти в каталог home надо написать cd /home.

- Для просмотра содержимого каталога используется команда ls. Например,

чтобы отобразить содержимое текущей директории с добавлением к именам символов, характеризующих их тип, надо написать ls -F.

- Команда du позволяет определить размер файла или каталога, применяется вместе с дополнительными операторами. Например, df –h — представляет данные о размере в удобном для восприятия формате.

- Команда mkdir создаёт новую директорию. Например, если ввести сочетание mkdir –p можно создать полную структуру подкаталогов. Команда rm отвечает за удаление папок и файлов. Например, для рекурсивного удаления используется сочетание rm -r.

- Команда chmod изменяет разрешения доступа к файлу. Например, чтение r, изменение w и запуск x.

- Команда history показывает ранее введённые пользователем команды.

3. Файловая система - часть операционной системы, которая обеспечивает чтение и запись файлов на дисковых носителях информации. Файловая система устанавливает физическую и логическую структуру файлов, правила их создания и управления ими, а также сопутствующие данные файла и идентификацию. Конкретная файловая система определяет размер имени файла, максимальный возможный размер файла. Операционная Система Linux поддерживает множество файловых систем. Например, рассмотрим как работают файловая система Ext2. Данные сначала кэшируются и только потом записываются на диск, чем достигается высокая производительность.

4. Посмотреть список всех смонтированных файловых систем можно с помощью команды mount без параметров.

5. SIGINT - самый безобидный сигнал завершения, означает Interrupt. Он отправляется процессу, запущенному из терминала с помощью сочетания клавиш Ctrl+C. Процесс правильно завершает все свои действия и возвращает управление.