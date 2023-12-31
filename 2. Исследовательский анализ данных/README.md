# Исследовательский анализ данных

## Описание проекта
В текущей работе исследуем данные сервиса Яндекс.Недвижимость — архив объявлений за несколько лет о продаже квартир в Санкт-Петербурге и соседних населённых пунктах.

## Инструменты
*Python*
*Pandas*
*Matplotlib*
*Визуализация данных*
*Исследовательский анализ данных*
*Предобработка данных*

## Выводы
- Был проведен первичный анализ данных
- Пропущенные значения были заполнены медианными значениями, приведены к единообразию названия одних и тех же населенных пунктов
- Устранены дубликаты
- Определены быстрые и долгие продажи. Значения ниже 25% можно считать быстрыми продажами, что соотв-т 44 дням. Значения выше 75% можно считать долгими продажами, что соотв-т 223 дням.
- Для столбца типы этажей 'type_floor': первый этаж занимает самую минимальную стоимость, последний этаж самый дорогой, а другие этажи занимают промежуточное положение и их значение "прижато" к значению последнего этажа.
- Для столбца 'day_week' выгодными днями для покупки являются: 0, 1, 4 и 6, дни недели.
- Для столбца 'month' выгодными месяцами для покупки являются: 2, 3, 6, 8, 10 и 11.
- Также была посчитана средняя цена одного квадратного метра в 10 населённых пунктах с наибольшим числом объявлений.
- Населенные пункты с самыми дорогими кв.м.: Санкт-Петербург - 114849 руб и Пушкин - 103126 руб.
- Населенные пункты с самыми дешевыми кв.м.: Выборг - 58142 руб и Всеволожск - 68654 руб.
- Вычислена средняя цена каждого километра в Санкт-Петерубрге: Отчетлива видная отрицательная тендеция цены недвижимости при росте расстояния (км) от центра города. Наблюдается резкий рост при приближении к значению '0', т.е. центру города. Чем дальше от центра города, тем более цена стремится к горизонтальной линии, т.е. как таковой корреляции от значения 15 км от центра города практически нет. Если не учитывать некоторые выбросы после 40 км и 55 км.

## Статус
Проект закончен.



