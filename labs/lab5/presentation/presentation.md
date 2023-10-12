---
## Front matter
lang: ru-RU
title: Лабораторная работа №5
subtitle: Дискреционное разграничение прав в Linux. Исследование влияния дополнительных атрибутов
author:
  - Дорофеева Алёна Тимофеевна
institute:
  - Российский университет дружбы народов им. Патриса Лумумбы, Москва, Россия
date: 7 октября 2023

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Дорофеева Алёна Тимофеевна
  * студент группы НПИбд-01-20
  * Российский университет дружбы народов им. Патриса Лумумбы
  * [1032201392@pfur.ru](mailto:1032201392@pfur.ru)
  * <https://github.com/DorofeevaAT>

:::
::: {.column width="30%"}

:::
::::::::::::::

# Вводная часть

## Актуальность

- Необходимость понимания возможножностей, предоставляемых различными правами и атрибутами доступа для пользователей. 

## Объект и предмет исследования

- Применение SetUID-, SetGID- и Sticky-битов.

## Цели и задачи

- Изучить на практике действие SetUID-, SetGID- и Sticky-битов.

## Материалы и методы

- Командная строка ОС Linux

# Процесс выполнения работы

## Создание программы simpleid.c

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![](image/3.png)

## Выполнение программы simpleid.c  

![](image/4.png)

## Программа simpleid2.c

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![](image/5.png)

:::
::: {.column width="50%"}

## Изменение прав доступа

![](image/6.png)
![](image/7.png)

## Выполнение программы simpleid2.c

![](image/8.png)

## Назначение SetGID-бита

![](image/9.png)

## Запуск программы

![](image/10.png)

## Программа readfile.c

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![](image/11.png)

## Смена прав доступа

![](image/12.png)

![](image/13.png)

## Добавление SetUID-бита

![](image/14.png)

## Попытка чтения файла readfile.c

![](image/15.png)

## Попытка чтения файла /etc/shadow

![](image/16.png)

## Проверка наличия STICKY-бита на директории tmp и создание тестового файла

![](image/17.png)

![](image/18.png)

## Попытка дозаписи и записи в файл и его удалениие

![](image/19.png){width=70%}

![](image/20.png){width=70%}

## Удаление STICKY-бита

![](image/21.png)

## Попытка дозаписи и записи в файл и его удаление

![](image/22.png)

![](image/23.png)

# Результаты работы

- Изучила на практике действие SetUID-, SetGID- и Sticky-битов.

# Вывод

Изучила механизмы изменения идентификаторов, применения SetUID- и Sticky-битов. Получила практические навыки работы в консоли с дополнительными атрибутами. Рассмотрела работы механизма смены идентификатора процессов пользователей, а также влияние бита Sticky на запись и удаление файлов.

[def]: https://github.com/DorofeevaAT