# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #4 выполнил(а):
- Соловьева Ольга Павловна
- РИ-230942

Отметка о выполнении заданий (заполняется студентом):

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | * | 20 |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

## Цель работы
Реализовать принцип работы перцептрона, визуализировать ход его обучения и результаты работы.


## Задание 1
### в проекте Unity реализовать перцептрон, который умеет производить вычисления:

### OR | дать комментарии о корректности работы

### AND | дать комментарии о корректности работы

### NAND | дать комментарии о корректности работы

### XOR | дать комментарии о корректности работы


Реализовано в проекте Unity (на всякий случай Unitypackage представлен в файлах репозитория), для каждого из операторов отдельный объект в сцене.

При проверке каждый из реализованных операторов, кроме XOR, работает корректно и выдает нужные результаты. Для XOR не хватило даже 100 эпох обучения, при нескольких запусках он дает только 2 правильных ожидаемых значения. 


## Задание 2
### Построить графики зависимости количества эпох от ошибки  обучения. Указать от чего зависит необходимое количество эпох обучения.

![task 2](https://github.com/kurlyushonok/DA-in-GameDev-lab4/blob/main/graphs/AND.png)

![task 2](https://github.com/kurlyushonok/DA-in-GameDev-lab4/blob/main/graphs/NAND.png)

![task 2](https://github.com/kurlyushonok/DA-in-GameDev-lab4/blob/main/graphs/OR.png)

![task 2](https://github.com/kurlyushonok/DA-in-GameDev-lab4/blob/main/graphs/XOR.png)


В основном количество эпох зависит от типа оператора, для которого обучаем перцептрон. Для AND и NAND требуется больше эпох, чем на OR.


## Задание 3
### Построить визуальную модель работы перцептрона на сцене Unity.

Реализовано в проекте Unity с помощью двух кубов. На каждый из кубов можно навесить объект нужного перцептрона и в инспекторе указать номер входа для того результата, который мы хотим визуализировать (отсчет начинается с 0). При взаимодействии и в завимимости от исходных входных значений кубы меняют цвета - белый, если 0, черный, если 1.


## Выводы

Реализованный перцептрон довольно быстро обучается для операторов OR, AND и NAND, но при этом довольно плохо работает с XOR. В среднем ему надо 7-8 эпох обучения для корректной работы, что представлено на полученных графиках. В процессе обучения total errors может не только уменьшаться от эпохи к эпохе, но и увеличиваться. Также было реализовано визуальное представление для одного из входов перцептрона с помощью двух кубов.


## Powered by

**BigDigital Team: Denisov | Fadeev | Panov**
