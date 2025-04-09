# АНАЛИЗ ОБРАЗОВАТЕЛЬНЫХ МЕТРИК 
## Стек:
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Numpy](https://img.shields.io/badge/numpy-3670A0?style=for-the-badge&logo=numpy&logoColor=ffdd54)

Продакт-менеджер попросил вас проанализировать поведение студентов на курсах, предметах и экзаменах онлайн-школы и ответить на следующие вопросы:

1. Сколько студентов успешно сдали только один курс? (Успешная сдача — это зачёт по курсу на экзамене)

2. Найдите и отсортируйте id экзаменов в рамках курса по возрастанию уровня завершаемости*.


3. Выявите самые популярные предметы (ТОП-3) по количеству регистраций на них.


4. Выявите предметы с самым большим оттоком (ТОП-3).


5. Используя pandas, в период с начала 2013 по конец 2014 выявите семестр с самой низкой завершаемостью курсов.


6. Используя pandas, в период с начала 2013 по конец 2014 выявите семестр с самыми долгими средними сроками сдачи курсов.


7. Часто для качественного анализа аудитории используют подходы, основанные на сегментации. Используя python, постройте адаптированные RFM-кластеры студентов, чтобы качественно оценить свою аудиторию. В адаптированной кластеризации можно выбрать следующие метрики:

    * R — среднее время сдачи одного экзамена,

    * F — завершаемость курсов,

    * M — среднее количество баллов, получаемое за экзамен.

Для каждого RFM-сегмента постройте границы метрик recency, frequency и monetary для интерпретации этих кластеров. Описание подхода можно найти тут.

     7.1. Чему равна минимальная граница по recency?
     7.2. Чему равна максимальная граница по recency?
     7.3. Чему равна минимальная граница по monetary?
     7.4. Чему равна максимальная граница по monetary?
     7.5. Сколько клиентов попадут в кластер 232?

Используйте логику:

    a) по recency можно получить 2, если значение recency меньше либо равно,  медиане по recency. В остальных случаях — 1.

    b) по frequency можно получить 1, если значение frequency меньше 50. Можно получить 2, если значение по frequency меньше 100. Можно получить 3 в остальных случаях.

    c) по monetary можно получить 1, если значение monetary меньше 40. Можно получить 2, если значение по monetary меньше либо равно 80. Можно получить 3 в остальных случаях.

Для решения задачи проведите предварительное исследование данных и сформулируйте, что должно считаться курсом. Обосновать свой выбор вы можете с помощью фактов сдачи экзаменов, распределения студентов и уникального идентификатора курса.

