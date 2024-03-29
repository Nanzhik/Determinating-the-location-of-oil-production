# Определение места для бурения новой скважины

[ipynb](https://github.com/Nanzhik/Determinating-the-location-of-oil-production/blob/main/Determinating-the-location-of-oil-production.ipynb)

## Описание проекта

**Заказчик:** добывающая компания «ГлавРосГосНефть».   

**Задача:** решить, где бурить новую скважину. 

**Исходные данные:** пробы нефти в трёх регионах. Характеристики для каждой скважины в регионе уже известны. Данные синтетические: детали контрактов и характеристики месторождений не разглашаются. 

Необходимо построить модель для определения региона, где добыча принесёт наибольшую прибыль. Проанализировать возможную прибыль и риски техникой *Bootstrap*.

## Навыки и инструменты

* **python**
* **matplotlib**
* **seaborn**
* **numpy**
* **ptitprince**
* sklearn.linear_model.**LinearRegression**

## Вывод

* Изучены исходные данные и их распределения, выявлены зависимости между столбцами;
* Построена модель предсказания среднего объема запасов ресурсов в новых скважинах;
* Посчитан объем запасов сырья для безубыточной разработки - 111.11 тыс.баррелей. Прдсказанные средние объемы запасов сырья каждого региона оказались ниже данного значения;
* Выбраны скважины с самыми высокими оценками значений запасов;
* Определен регион с максимальной суммарной прибылью отобранных скважин.  

Таким образом, единственным регионом, удовлетворяющим заданному условию вероятности убытков оказался второй регион (1%). Также только у второго региона отсутствует риск получения отрицательной прибыли, в то время как у первого и третьего региона существует возможность уйти в "минус" более 100 млн.руб.
