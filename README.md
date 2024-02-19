# Project_3_Статистические_тесты_Практика
PROJECT_3_EDA. Исследование на основе данных о зарплатах в сфере Data Science за 2020–2022 годы.
# Проект 3. HR-агенство

## Оглавление

1. [Описание проекта.](https://github.com/Petrleon85/Project_3_EDA_practic/blob/main/README.md#описание-проекта)

1. [Проектный кейс.](https://github.com/Petrleon85/Project_3_EDA_practic/blob/main/README.md#проектный-кейс)

1. [Результат.](https://github.com/Petrleon85/Project_3_EDA_practic/blob/main/README.md#результат)

1. [Выводы.](https://github.com/Petrleon85/Project_3_EDA_practic/blob/main/README.md#выводы)

### Описание проекта
---

К вам как опытному дата-сайентисту обратилась HR-агенство. Компания хочет провести исследование на основе данных о зарплатах в сфере Data Science за 2020–2022 годы и получить некоторые выводы.

Агенство хочет ответить на следующие вопросы, касающиеся зарплат у специалистов Data Scientist:

1. Выяснить, какие факторы влияют на зарплату специалиста Data Scientist.
2. А также ответить на ключевые вопросы HR-агентства:
- Наблюдается ли ежегодный рост зарплат у специалистов Data Scientist?
- Как соотносятся зарплаты Data Scientist и Data Engineer в 2022 году?
- Как соотносятся зарплаты специалистов Data Scientist в компаниях различных размеров?
- Есть ли связь между наличием должностей Data Scientist и Data Engineer и размером компании?

Необходимо найти в данных интересные закономерности, также отметьте их в своём анализе.

### Проектный кейс

---

**Условие задачи**

* Выполнить задание согласно ноутбуку шаблону, выложенному на платформе. 
* По каждому заданию в ноутбук-шаблон добавить код и выводы.
* На каждый вопрос необходимо ответить с уровнем значимости $\alpha=0.05$.
* Продемонстрировать использование разных тестов для проверки статистической значимости сделанных выводов:

тесты для количественного признака:
для одной выборки;
для двух выборок;
для нескольких выборок;
тест для категориальных признаков.

**Метрика качества**

КРИТЕРИИ ОЦЕНИВАНИЯ (МАКСИМУМ — 12 БАЛЛОВ)

Загрузка и обработка данных (2 балла)

ОПИСАНИЕ КРИТЕРИЯ	БАЛЛЫ
Студент корректно загрузил данные.
Студент проверил датасет на наличие пропусков и дубликатов, а также на корректность типов данных столбцов.
Студент определил в данных неинформативные признаки, которые не будут участвовать в исследовании.
Студент классифицировал все признаки на числовые и категориальные.
Студент нашёл основные статистические характеристики для каждого из признаков.
2
Корректно выполнена только часть из пунктов.	1
Ни один из пунктов не выполнен корректно.	0
Разведывательный анализ данных (4 балла)

2.1. Визуальный анализ данных (2 балла)

ОПИСАНИЕ КРИТЕРИЯ	БАЛЛЫ
Студент выполнил визуальный анализ данных.
Сделан базовый анализ для каждого признака, участвующего в исследовании:
для числовых признаков построены гистограммы, иллюстрирующие распределения;
для категориальных признаков определено количество записей для каждой категории и построены соответствующие визуализации.
Студент создал корректные визуализации, которые демонстрируют влияние каждого из признаков, участвующих в исследовании, на зарплату по всем наименованиям Data Scientist или на зарплату по всем должностям.
Студент на основе визуального анализа дал первичные ответы на поставленный в задании вопрос: «Какие факторы влияют на заработную плату?».
2
Корректно выполнена только часть из пунктов, или визуальный анализ выполнен не для всех признаков.	1
Визуальный анализ данных не выполнен.	0
2.2. Статистический анализ данных (2 балла)

ОПИСАНИЕ КРИТЕРИЯ	БАЛЛЫ
В исследовании студент подтвердил или опроверг свои первичные гипотезы, полученные на этапе визуального анализа, с помощью статистических тестов:
Студент корректно сформулировал нулевые и альтернативные гипотезы на основе поставленных бизнес-вопросов.
Студент правильно выбрал статистический тест для каждой из гипотез, предварительно проверив условие его применения (там, где это необходимо):
проверка на нормальность;
проверка равенства дисперсий в группах.
Студент успешно протестировал данные, продемонстрировав владение различными статистическими тестами:
тесты для количественного признака:
для одной выборки;
для двух выборок;
для нескольких выборок;
тест для категориальных признаков.
2
Корректно выполнена только часть из пунктов, или статистический анализ выполнен не для всех признаков.	1
Статистический анализ данных не выполнен.	0
Соответствие выводов бизнес-вопросам (4 балла)

ОПИСАНИЕ КРИТЕРИЯ	БАЛЛЫ
Студент привёл развёрнутые и обоснованные ответы по каждому вопросу:
Наблюдается ли ежегодный рост зарплат у специалистов Data Scientist?
Как соотносятся зарплаты Data Scientist и Data Engineer в 2022 году?
Как соотносятся зарплаты специалистов Data Scientist в компаниях различных размеров?
Есть ли связь между наличием должностей Data Scientist и Data Engineer и размером компании?
Представленные выводы корректны и соответствуют результатам, полученным в ходе статистического анализа.

Cуммарно 4 балла (по 1 баллу за каждый вывод по гипотезам)
Дополнительное исследование (2 балла)

ОПИСАНИЕ КРИТЕРИЯ	БАЛЛЫ
Студент самостоятельно корректно сформулировал минимум две дополнительных бизнес-гипотезы о влиянии факторов на заработную плату специалистов и для каждой гипотезы:
представил визуальный анализ данных;
произвёл статистическое тестирование;
сделал верные, соответствующие бизнес-вопросам выводы по полученным результатам.
2
Студент самостоятельно сформулировал только одну дополнительную бизнес-гипотезу и выполнил все пункты для её подтверждения/опровержения.

ИЛИ

Студент самостоятельно сформулировал две или более дополнительных бизнес-гипотезы, но не выполнил / выполнил некорректно часть пунктов для их подтверждения/опровержения.	1
Студент не стал выполнять дополнительное исследование.	0
Оформление исследования (2 балла)

ОПИСАНИЕ КРИТЕРИЯ	БАЛЛЫ
Студент качественно оформил решение задачи:
Описана постановка задачи.
На протяжении всего исследования прослеживается логика, ноутбук имеет понятную структуру, разделён на части заголовками.
Есть промежуточные выводы.
Все визуализации имеют подписи к осям и заголовки и соответствуют стандартам оформления.
Сделан финальный вывод по исследованию.
Код студента понятный, оформлен по стандартам PEP-8 и сопровождён комментариями.
2
Выполнена только часть из пунктов.	1
Ноутбук содержит только код.	0
Задание, оцениваемое ментором
* Получить обратную связь от команды курса.

**Что практикуем**

* базовый анализ структуры данных;
* преобразование данных;
* разведывательный анализ;
* очистка данных.


⬆️[к оглавлению](https://github.com/Petrleon85/Project_3_EDA_practic/blob/main/README.md#оглавление)

### РЕЗУЛЬТАТ

---

Проект загружен на [GitHub](https://github.com/Petrleon85/Project_3_EDA_practic.git), обеспечена воспроизводимость кода:

*   [Leontev_EDA_4_Статистические_тесты_Практика.ipynb]((Leontev_EDA_4_Статистические_тесты_Практика.ipynb)) - ноутбук-шаблон с решениями заданий;
*   [requirements.txt](requirements.txt) - актульные версии библиотек на момент подготовки проекта;
*   [обратная связь от ментора.]
*  

⬆️[к оглавлению](https://github.com/Petrleon85/Project_3_EDA_practic/blob/main/README.md#оглавление)

### ВЫВОДЫ

*   Средний размер зарплат специалистов Data Scientist в 2022 году статистически больше, чем размер размер зарплат специалистов Data Scientist в 2021 году.
*   Размер зарплатных выплат специалистов Data Scientist отличается в зависиомсти от размера компании.
*   У нас нет оснований отвергнуть нулевую гипотезу, а значит размер зарплат для специалистов Data Scientist статистически больше либо равен размеру зарплат специалистов Data Engineer в 2022 году.
*   Существует статистически значимая взаимосвязь между специалистами Data Scientist и Data Engineer и размером компании.
*   Средний размер зарплат специалистов Data Engineer в 2022 году статистически больше, чем размер размер зарплат специалистов Data Engineer в 2021 году.
*   Размер заработных выплат отличается в разных регионах: CA, DE, GB, IN.


Исходя из анализа данных, есть основания полагать, что на денежное содержание специалистов Data Scientist влияют следующие факторы:
*   *experience_level* — опыт работы;
*   *employment_type* — 	тип трудоустройства для этой роли;
*   *job_title* — 	роль, в которой соискатель работал в течение года;
*   *company_location* — 	страна главного офиса работодателя или филиала по контракту в виде кода страны ISO 3166;
*   *company_size* — 	среднее количество людей, работавших в компании в течение года.

Выводы по проекту изложены в ноутбуке-шаблоне.

**Проблемные моменты**


**Полезный опыт**

Для форматирования кода удобно использовать расширение VSCode [Black Formatter](https://marketplace.visualstudio.com/items?itemName=ms-python.black-formatter).



⬆️[к оглавлению](https://github.com/Petrleon85/Project_3_EDA_practic/blob/main/README.md#оглавление)
