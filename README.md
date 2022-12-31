
# Очистка и анализ данных сервиса HeadHunter.ru на Python

![Очистка данных сервиса HeadHunter](https://iprodvinem.com/wp-content/uploads/2021/04/headhunter-hh.ru-sayt-po-poisku-raboty-870x400.png)

## Оглавление

1. [Описание проекта и его этапов](#описание-проекта)
2. [Описание данных](#описание-данных)
3. [Зависимости и файлы](#используемые-зависимости)
4. [Установка проекта](#установка-проекта)
5. [Использование проекта](#использование)
6. [Авторы](#авторы)
7. [Выводы](#выводы)

## Описание проекта

В нашем проекте по Data Science мы работаем с базой данных резюме соискателей работы сервиса HeadHunter.ru. Наша цель - предоставить работодателям более точную информацию о кандидатах на вакансии.

## Основные этапы проекта

### **Анализ структуры данных**

Этап анализа структуры данных в проекте по Data Science предназначен для изучения характеристик и свойств набора данных, которым мы работаем. В этом этапе мы стараемся ответить на следующие вопросы:

* Какие типы данных содержатся в наборе данных?
* Какие признаки (столбцы) присутствуют в наборе данных?
* Есть ли пропущенные значения в наборе данных?
* Какие преобразования необходимо произвести над данными для возможности их дальнейшего анализа?

### **Преобразование данных**

Этап преобразования данных в проекте по Data Science направлен на изменение формата, структуры или типа данных в наборе данных, чтобы сделать их более подходящими для дальнейшего анализа или машинного обучения.
В этом этапе мы можем выполнять различные операции над данными, такие как:

* Вычленение полезной информации из имеющихся признаков (Пол, Возраст, готовность к определенному режиму работы, предпочтения по рабочему графику)
* Разделение соединенных вместе признаков для удобного анализа в дальнейшем
* Унификация единиц измерения признаков (например Заработная плата)

### **Исследование зависимостей в данных**

Этап исследования зависимостей в данных в проекте по Data Science направлен на обнаружение связей между различными признаками в наборе данных. Это может быть полезно для того, чтобы понять, какие признаки влияют на результаты и какие признаки могут быть использованы в моделях машинного обучения для прогнозирования или классификации.

В этом этапе мы путем построения графиков (scatter plots, box plots, etc.) и примененная статистического анализа стремимся ответить на следующие вопросы:

* Как распределены значения в каждом признаке?
* Существуют ли зависимости между различными признаками?

### **Очистка данных от пропусков и дубликатов**

Этап очистки данных от пропусков и дубликатов в проекте по Data Science направлен на устранение некорректных или неполных значений в наборе данных. Это важно, так как пропущенные или дублирующиеся данные могут существенно искажать результаты анализа и вызывать неточности в моделях машинного обучения.

**О структуре проекта:**

* [data](./data) - папка с исходными табличными данными
* [graphs](./graphs) - папка с сохраненными графиками по итогам анализа
* [Project-1_HH_data.ipynb](./Project-1_HH_data.ipynb) - jupyter-ноутбук, содержащий основной код проекта

## Описание данных

В этом проекте используются данные о резюме (CV), предоставленных сервисом по поиску работы и работников [HeadHunter.ru](https://hh.ru/).

Данные содержат в себе сведения о более чем 44 тысячах соискателей, в том числе о желаемой заработной плате, городе проживания, опыте работы, возраста и пола соискателя.

## Используемые зависимости

* Python (3.10):
  * [numpy (1.23.2)](https://numpy.org)
  * [pandas (1.4.4)](https://pandas.pydata.org)
  * [matplotlib (3.6.2)](https://matplotlib.org)
  * [seaborn (0.12.1)](https://seaborn.pydata.org)
  * [plotly (5.11.0)](https://plotly.com/graphing-libraries/)

## Установка проекта

```Git
git clone https://github.com/shohart/Headhunter-Project1.git
```

## Использование

Вся информация о работе представлена в jupyter-ноутбуке *Project-1_HH_data.ipynb.*

Датасеты можно скачать [тут](https://drive.google.com/drive/folders/1KcT76dvZhzMB8eRu-6TgktZhq2vYkBe_?usp=sharing)

## Авторы

* [Aleksei Bykov](https://www.linkedin.com/in/aleksei-bykov-vilnius/)

## Выводы

В результате проекта Анализа данных резюме с сайта hh.ru были успешно реализованы следующие этапы:

* Анализ структуры данных. Была произведена оценка типа и размера данных, обнаружены некорректные и незаполненные значения.

* Преобразование данных. Были приведены типы данных к нужным форматам, отброшена лишняя информация, определены новые признаки, пригодные для анализа.

* Исследование зависимостей в данных. Были построены графики и выполнен корреляционный анализ для обнаружения связей между различными признаками.

* Очистка данных от пропусков и дубликатов. Были удалены некорректные и повторяющиеся значения, что позволило улучшить точность анализа и избавиться от искажающего влияния на результаты.

* Отдельно стоит отметить существенное уменьшение размера датасета (с почти 500 мб до не более чем 14 мб), при существенном повышении общей пригодности и информативности данных.

В результате проведенных операций датасет пригоден для дальнейшего использования в целях Data Science.
