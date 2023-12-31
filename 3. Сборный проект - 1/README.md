# Сборный проект - 1

## Описание проекта
Имеется датафрейм интернет-магазина «Стримчик», который продаёт по всему миру компьютерные игры.
Из открытых источников доступны исторические данные о продажах игр, оценки пользователей и экспертов, жанры и платформы (например, Xbox или PlayStation). Необходимо выявить определяющие успешность игры закономерности. Это позволит сделать ставку на потенциально популярный продукт и спланировать рекламные кампании.

## Инструменты
*Python*
*Pandas*
*NumPy*
*Matplotlib*
*предобработка данных*
*исследовательский анализ данных*
*описательная статистика*
*проверка статистических гипотез*

## Выводы
- Отобрал топ-10 платформ по суммарным продажам. Платформы, существующие в 2016 году стали: `'PS4', 'PS3', '3DS', 'X360', 'Wii'`. `Актуальный период получился с 2013 по 2016 гг`.

- Определил лидера по продажам в актуальном периоде с 2013-2016 гг., им стала `'PS4'`. На втором месте `'XOne'`, следом `'PS3'`. Вторым заметным конкурентом, который разделит часть рынка с `'PS4'` можно выделить `'XOne'`.

- Построил график «ящик с усами» по глобальным продажам игр в разбивке по платформам. Самая высокая медиана и верхний квартиль у `'X360'`. Следом идут `'PS4'`, `'Wii'` и `'XOne'`. Аутсайдерами же в отчетном периоде оказались: `'PSV' и 'PSP'`.

- Рассмотрел, как влияют на продажи внутри одной популярной платформы отзывы пользователей и критиков и сравнили с продажами игр на других платформах. Коэффициенты корреляции отн-о критиков выше, чем коэф. корреляции для пользователей. Из чего можно сделать вывод, что присутствует некоторая корреляция между суммарными продажами и оценкой критиков. А в случае между суммарными продажами и оценкой пользователей корреляции нет, если она и есть, то очень не большая.

- Рассмотрел общее распределение игр по жанрам. Самый высокий верхний квартиль и медиана у `'Shooter'`. Следом идут, примерно, на одном уровне `'Sports' и 'Platform'`. Самые же малочисленные жанры: `'Strategy', 'Adventure', 'Puzzle'`.

Рассмотрел портрет пользователей по каждому региону: `Северная Америка, Европа, Япония`.
    
`SA`
1. Для региона Северной Америки две самые популярные конкурирующие платформы, которые выше медианы `'PS4'` и `'XOne'`. Прям на медиане располагается `'X360'` 82 (млн. копий).
2. Для региона Северной Америки самые популярные жанры: `'Action'`, `'Shooter'`. Прям на медиане располагается `'Sports'` 65.27.
3. Более всех влияют на продажи два рейтинга: `'M', 'no_rating' и 'E'` (располагается прямо на медиане). Замыкает четвёрку рейтинг `'E10+'`.
    
`EU`
1. Для региона Европа две самые популярные платформы `'PS4' и 'PS3'`. На третьем месте платформа, которая располагается на медиане `'XOne'` - 51.59 (млн. копий).
2. Для региона Европа самые популярные жанры: `'Action', 'Shooter' и 'Sports'`. `'Sports'` 60.52 (млн. копий) располагается на медиане 61 (млн. копий).
3.  Более всех влияют на продажи два рейтинга: `'М', 'E' и 'no_rating'` 78.91 (млн копий) находится прям ровно на медиане 79.
    
`JP`
1. Для региона Япония три самые популярные платформы `'3DS', 'PS3', 'PS4'`. `'PS4'` находится на медиане 19 (млн копий) с значением 18.59 (млн копий).
2. Для региона Япония самые популярные жанры: `'Role-Playing', 'Action'` и прям на медиане находится `'Misc'` со значением 9.20 (млн. копий) на медиане 9 (млн. копий).
3.  Более всех влияют на продажи `'no_rating'`. Следом `'T'`. Замыкает тройку рейтинг `'E'`, его значение 15.14 (млн копий) находится на медиане 15 (млн копий).

Проверил гипотезы о равенстве средних пользовательский рейтинга платформ `Xbox One` и `PC`.  
Было получено p-значение: `0.14759594013430463`, что существенно больше *`alpha=0.05`*. Из этого можно сделать вывод, что данные *не противоречат* нулевой гипотезе: средние рейтинги по платформам равны, поэтому мы её не отвергаем.

Проверил гипотезу, что пользовательские рейтинги жанров `Action и Sports` различаются.  
После проверки с точностью *`alpha=0.05`* мы получили очень низкое значение p-value, равное `1.446e-20`. Это значит, что мы имеем основание отбросить нулевую гипотезу и принять альтернативную: пользовательские рейтинги жанров Action и Sports *имеют статистически значимые различия*.

## Статус
Проект закончен.



