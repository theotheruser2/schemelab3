<!-- федеральное государственное автономное образовательное учреждение высшего образования
«Национальный исследовательский университет ИТМО» -->

# Лабораторная работа №3 &laquo;Функциональная схемотехника&raquo;

Выполнили студенты группы P33113:  Доморацкий Э.А., Юров М.А.

Преподаватель: Тищук Б.Ю.

Санкт-Петербург, 2021

Цель работы
=======

Получить навыки разработки цифровых устройств на базе программируемых логических интегральных схем (ПЛИС).


Схема портов ввода-вывода
=======================

![](./scheme.png)

Алгоритм работы пользователя
===========================



Код исходной схемы
========================

Репозиторий: https://github.com/theotheruser2/schemelab3  

`sqrt.v` - блок вычисления квадратного корня\
`a_sqrtb.v` - схема для вычисления значения функции

Код разработанного тестового окружения 
=======================================

`ab_tb.v` - тестирование блока вычисления квадратного корня\
`s_test.v` - тестирование работы схемы в целом


Временная диаграмма
===================

Сигналы подаются с частотой 100 МГц. На рассчёт одного значения уходит 580 нс.

![](./time1.png)


Потребление ресурсов
====================

Полученные на основе симуляции данные об использовании ресурсов устройства, энергопотреблении, температуре:

![](./stat.png)

Вывод
=====

В результате работы была создан арифметический блок для вычисления значений функции `y = a * √b`, описанный на RTL-уровне при помощи языка Verilog HDL, было разработано тестовое окружение.
