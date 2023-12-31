# Анализ данных платформы Kickstarter: определение наиболее успешных категорий проектов и прогнозирование будущих результатов

## Описание проекта

Наш проект посвящен анализу данных платформы Kickstarter. Мы взяли датасет `kickstarter_projects.csv`, который содержит информацию о проектах, запущенных на платформе Kickstarter. Наша цель - провести различные анализы на основе этих данных и выявить тенденции, тренды и факторы, которые влияют на успех проектов на платформе Kickstarter.
Представим, что сейчас начало 2018 года, и нам нужно выяснить, какие проекты будут успешны в будущем, проанализивав данные за предыдущие годы.

**Цель проекта:**
- изучение распределения проектов по категориям и определение наиболее популярных категорий проектов на платформе;
- определение оптимальной суммы для достижения целей проектов в различных категориях;
- анализ региональных различий и определение наиболее популярных стран для старта проекта;
- изучение трендов и изменений, происходящих на платформе;
- подбор критериев, на которые нужно обратить внимание, чтобы гарантировать успех проекта в будущем.

## Выводы:
- проекты размещаются в 21 странах:
    - 80% США (37.68% успешных);
    - 9.2% Великобритания (36.26% успешных);
    - 4% Канада (28.67% успешных);
    - 2.1% Австралия (26.29% успешных);
    - 1.1% в Германии (23.02% успешных) и др.
- проекты имеют 5 состояний:
    - 52.7% Failed;
    - 35.7% Successful;
    - 10.3% Canceled;
    - 0.7% Live;
    - 0.5% Suspended.
- проекты делятся на 14 категорий, топ 5 по количеству успешных:
    - Music	(48.81% успешных);
    - Film & (Video 37.80% успешных);
    - Games (36.18% успешных);
    - Publishing (31.43% успешных);
    - Art (41.22% успешных).
- проекты делятся на 159 подкатегорий, топ 5 по количеству успешных:
    - Product Design (36.86% успешных);
    - Tabletop Games (56.45% успешных);
    - Shorts (54.15% успешных);
    - Music (47.71% успешных);
    - Documentary (36.78% успешных).
- в среднем сбор средств длился 29 дней;
- количество проектов активно увеличивалось до 2015 года, так же увеличивалось и кол-во неудачных проектов, после 2015 года запуск новых проектов стал замедляться;
- в 2014 году начался "хайп", пик которого пришелся на 2015 год, было запущено много проектов, большинство из которых не смогли собрать необходимую сумму средств;
- количество успешных проектов с 2013 по 2017 годы +- одинаковые;
- за 2015-2017 годы в США больше всего проектов запускаются в начале года (пик в марте), однако, успешных проектов больше осенью (пик в октябре).

**Для инвесторов** 

Чтобы выбрать тип наиболее успешных проектов, мы оставили данные США за последние 3 года, а так же убрали проекты, которые еще собирают средства. У нас осталось 122792 проекта, разделив их на 4 равные доли, учитывая сумму денег, необходимую автору для завершения проекта, провели исследование и выявили подкатегории проектов, которые из года в год показывают наибольший результат успешности:
[Подробнее](https://github.com/dintempl/pet_projects_DA/blob/main/%D0%90%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%20%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85%20%D0%BF%D0%BB%D0%B0%D1%82%D1%84%D0%BE%D1%80%D0%BC%D1%8B%20Kickstarter/kickstarter_projects_analysis.ipynb)

## Использованные библиотеки
```
pandas
seaborn
numpy
matplotlib
datetime
```
