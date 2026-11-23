---
jupyter:
  jupytext:
    text_representation:
      extension: .md
      format_name: markdown
      format_version: '1.3'
      jupytext_version: 1.19.5
  kernelspec:
    display_name: Python 3 (ipykernel)
    language: python
    name: python3
---

# Сводная таблица тем курсовых работ

Описание каждой темы — в файле [`topics_ml.md`](topics_ml.md).

## Уровни сложности

| Уровень | Описание |
|---|---|
| 🟢 1 — базовая | До 2 000 строк, признаки числовые, пропусков мало |
| 🟡 2 — средняя | 2 000–200 000 строк, есть категории, пропуски, дисбаланс классов |
| 🔴 3 — сложная | 200 000+ строк, временные ряды, текст или изображения, либо сильный дисбаланс |

## Группа 1. Классификация на табличных данных

| № | Тема | Тип задачи | Набор данных | Объём | Уровень |
|---|---|---|---|---|---|
| 1 | Предсказание годового дохода по данным переписи | Бинарная классификация | [Adult, UCI id=2](https://archive.ics.uci.edu/dataset/2) | 48 842 × 14 | 🟡 |
| 2 | Отклик на маркетинговую кампанию банка | Бинарная классификация, дисбаланс 11 % | [Bank Marketing, UCI id=222](https://archive.ics.uci.edu/dataset/222) | 45 211 × 16 | 🟡 |
| 3 | Прогноз дефолта по кредитной карте | Бинарная классификация, дисбаланс 22 % | [Default of Credit Card Clients, UCI id=350](https://archive.ics.uci.edu/dataset/350) | 30 000 × 23 | 🟡 |
| 4 | Одобрение кредитной заявки | Бинарная классификация, пропуски | [Credit Approval, UCI id=27](https://archive.ics.uci.edu/dataset/27) | 690 × 15 | 🟢 |
| 5 | Оценка кредитного риска (Statlog) | Бинарная классификация | [Statlog (German Credit), UCI id=144](https://archive.ics.uci.edu/dataset/144) | 1 000 × 20 | 🟢 |
| 6 | Прогноз банкротства компаний | Бинарная классификация, дисбаланс 3.8 % | [Taiwanese Bankruptcy Prediction, UCI id=572](https://archive.ics.uci.edu/dataset/572) | 6 819 × 95 | 🔴 |
| 7 | Прогноз отсева студентов | Многоклассовая классификация (3 класса) | [Predict Students' Dropout, UCI id=697](https://archive.ics.uci.edu/dataset/697) | 4 424 × 36 | 🟡 |
| 8 | Диагностический скрининг диабета | Бинарная классификация, большие данные | [CDC Diabetes Health Indicators, UCI id=891](https://archive.ics.uci.edu/dataset/891) | 253 680 × 21 | 🔴 |
| 9 | Диагностика ишемической болезни сердца | Бинарная классификация | [Heart Disease, UCI id=45](https://archive.ics.uci.edu/dataset/45) | 303 × 13 | 🟢 |
| 10 | Диагностика кожных заболеваний | Многоклассовая классификация (6 классов) | [Dermatology, UCI id=33](https://archive.ics.uci.edu/dataset/33) | 366 × 34 | 🟢 |
| 11 | Хроническая болезнь почек | Бинарная классификация, пропуски 30 % | [Chronic Kidney Disease, UCI id=336](https://archive.ics.uci.edu/dataset/336) | 400 × 24 | 🟢 |
| 12 | Прогноз исхода при гепатите | Бинарная классификация, дисбаланс 4:1 | [Hepatitis, UCI id=46](https://archive.ics.uci.edu/dataset/46) | 155 × 19 | 🟢 |
| 13 | Ишемия по данным ОФЭКТ сердца | Бинарная классификация | [SPECTF Heart, UCI id=96](https://archive.ics.uci.edu/dataset/96) | 267 × 44 | 🟡 |
| 14 | Выявление диабетической ретинопатии | Бинарная классификация | [Diabetic Retinopathy Debrecen, UCI id=329](https://archive.ics.uci.edu/dataset/329) | 1 151 × 19 | 🟡 |
| 15 | Классификация стадий заболеваний печени | Многоклассовая классификация (5 классов) | [HCV data, UCI id=571](https://archive.ics.uci.edu/dataset/571) | 615 × 12 | 🟡 |
| 16 | Локализация первичной опухоли | Многоклассовая классификация (4 класса) | [Primary Tumor, UCI id=83](https://archive.ics.uci.edu/dataset/83) | 339 × 17 | 🟡 |
| 17 | Детекция фишинговых сайтов | Бинарная классификация | [Phishing Websites, UCI id=327](https://archive.ics.uci.edu/dataset/327) | 11 055 × 30 | 🟡 |
| 18 | Фильтрация спама в почтовых ящиках | Бинарная классификация | [Spambase, UCI id=94](https://archive.ics.uci.edu/dataset/94) | 4 601 × 57 | 🟡 |
| 19 | Распознавание сортов фасоли | Многоклассовая классификация (7 классов) | [Dry Bean, UCI id=602](https://archive.ics.uci.edu/dataset/602) | 13 611 × 16 | 🟡 |
| 20 | Распознавание покерных комбинаций | Многоклассовая классификация, дисбаланс 100 000:1 | [Poker Hand, UCI id=158](https://archive.ics.uci.edu/dataset/158) | 1 025 010 × 10 | 🔴 |
| 21 | Различение сортов риса по признакам | Бинарная классификация | [Rice (Cammeo and Osmancik), UCI id=545](https://archive.ics.uci.edu/dataset/545) | 3 810 × 7 | 🟢 |
| 22 | Выявление диабета по данным NHANES | Бинарная классификация | [NHANES 2013–2014, UCI id=887](https://archive.ics.uci.edu/dataset/887) | 6 287 × 48 | 🟡 |
| 23 | Качество спермы и фертильность | Бинарная классификация, очень малый объём | [Fertility, UCI id=244](https://archive.ics.uci.edu/dataset/244) | 100 × 9 | 🟢 |


| № | Тема | Тип задачи | Набор данных | Объём | Уровень |
|---|---|---|---|---|---|
| 24 | Прогноз послеоперационных осложнений | Бинарная классификация | [Post-Operative Patient, UCI id=82](https://archive.ics.uci.edu/dataset/82) | 90 × 8 | 🟡 |
| 25 | Исход колики у лошадей | Бинарная классификация, пропуски | [Horse Colic, UCI id=47](https://archive.ics.uci.edu/dataset/47) | 368 × 27 | 🟡 |
| 26 | Диагностика заболеваний печени у пациентов Индии | Бинарная классификация, дисбаланс 3:1 | [ILPD, Indian Liver Patient Dataset, UCI id=225](https://archive.ics.uci.edu/dataset/225) | 583 × 10 | 🟡 |
| 27 | Диагностика ишемии по перфузии миокарда | Бинарная классификация | [SPECT Heart, UCI id=95](https://archive.ics.uci.edu/dataset/95) | 267 × 22 | 🟢 |
| 28 | Классификация стадий фиброза печени | Бинарная классификация, дисбаланс 13 % | [HCV data, UCI id=571](https://archive.ics.uci.edu/dataset/571) | 615 × 12 | 🟡 |
| 29 | Обнаружение масс в маммографии | Бинарная классификация | [Mammographic Mass, UCI id=161](https://archive.ics.uci.edu/dataset/161) | 961 × 5 | 🟢 |
| 30 | Классификация вариантов контрацепции | Многоклассовая классификация (3 класса) | [Contraceptive Method Choice, UCI id=30](https://archive.ics.uci.edu/dataset/30) | 1 473 × 9 | 🟢 |
| 31 | Диагностика гипертонии по ЭКГ плода | Многоклассовая классификация (3 класса) | [Cardiotocography, UCI id=193](https://archive.ics.uci.edu/dataset/193) | 2 126 × 21 | 🟡 |
| 32 | Скрининг расстройств аутистического спектра | Бинарная классификация, пропуски | [Autistic Spectrum Disorder Screening Data for Children, UCI id=419](https://archive.ics.uci.edu/dataset/419) | 292 × 20 | 🟡 |
| 33 | Выявление фиброза печени у египетских пациентов | Многоклассовая классификация (5 классов) | [Hepatitis C Virus (HCV) for Egyptian patients, UCI id=503](https://archive.ics.uci.edu/dataset/503) | 1 385 × 28 | 🟡 |
| 34 | Предсказание задержки сети в радиоастрономии | Бинарная классификация, дисбаланс 1.8:1 | [MAGIC Gamma Telescope, UCI id=159](https://archive.ics.uci.edu/dataset/159) | 19 020 × 10 | 🟡 |
| 35 | Диагностика заболеваний по маммографическим и клиническим данным | Бинарная классификация | [Breast Cancer Coimbra, UCI id=451](https://archive.ics.uci.edu/dataset/451) | 116 × 9 | 🟢 |
| 36 | Классификация урологических заболеваний | Многоклассовая классификация (4 класса) | [Acute Inflammations, UCI id=184](https://archive.ics.uci.edu/dataset/184) | 120 × 6 | 🟢 |
| 37 | Определение режима работы энергосетической системы | Бинарная классификация | [Electrical Grid Stability Simulated Data, UCI id=471](https://archive.ics.uci.edu/dataset/471) | 10 000 × 12 | 🟡 |
| 38 | Аппроксимация суточного профиля нагрузки электросети | Регрессия временного ряда | [Metro Interstate Traffic Volume, UCI id=492](https://archive.ics.uci.edu/dataset/492) | 48 204 часовых | 🔴 |
| 39 | Регрессионные модели длительности и выживаемости | Регрессия | [Liver Disorders, UCI id=60](https://archive.ics.uci.edu/dataset/60) | 345 × 5 | 🟢 |
| 40 | Факторы риска рака шейки матки | Бинарная классификация, пропуски | [Cervical Cancer (Risk Factors), UCI id=383](https://archive.ics.uci.edu/dataset/383) | 858 × 36 | 🔴 |
| 41 | Прогноз оттока абонентов телеком-оператора | Бинарная классификация, дисбаланс 23 % | [Iranian Churn, UCI id=563](https://archive.ics.uci.edu/dataset/563) | 3 150 × 13 | 🟡 |
| 42 | Предсказание покупки в интернет-магазине | Бинарная классификация, дисбаланс 18 % | [Online Shoppers Purchasing Intention, UCI id=468](https://archive.ics.uci.edu/dataset/468) | 12 330 × 17 | 🟡 |
| 43 | Обнаружение фишинговых сайтов | Бинарная классификация | [Website Phishing, UCI id=379](https://archive.ics.uci.edu/dataset/379) | 1 353 × 30 | 🟡 |
| 44 | Детекция занятости помещения | Бинарная классификация временных рядов | [Occupancy Detection, UCI id=357](https://archive.ics.uci.edu/dataset/357) | 20 560 измерений (1 мин) | 🟢 |
| 45 | Прогноз невыходов на работу по данным организации | Регрессия | [Absenteeism at work, UCI id=445](https://archive.ics.uci.edu/dataset/445) | 740 × 20 | 🟡 |
| 46 | Одобрение кредита | Бинарная классификация | [Statlog (Australian Credit Approval), UCI id=143](https://archive.ics.uci.edu/dataset/143) | 690 × 14 | 🟢 |
| 47 | Прогноз банкротства компаний | Бинарная классификация, дисбаланс 6 % | [Polish Companies Bankruptcy, UCI id=365](https://archive.ics.uci.edu/dataset/365) | 10 503 × 65 | 🔴 |
| 48 | Оценка заполненности помещения | Бинарная классификация, датчики | [Room Occupancy Estimation, UCI id=864](https://archive.ics.uci.edu/dataset/864) | 10 129 × 7 | 🟡 |

## Группа 2. Регрессия

| № | Тема | Тип задачи | Набор данных | Объём | Уровень |
|---|---|---|---|---|---|
| 49 | Расход топлива автомобиля | Регрессия | [Auto MPG, UCI id=9](https://archive.ics.uci.edu/dataset/9) | 398 × 7 | 🟢 |
| 50 | Прочность бетона | Регрессия, нелинейная зависимость | [Concrete Compressive Strength, UCI id=165](https://archive.ics.uci.edu/dataset/165) | 1 030 × 8 | 🟢 |
| 51 | Нагрузки на отопление и охлаждение здания | Многомерная регрессия | [Energy Efficiency, UCI id=242](https://archive.ics.uci.edu/dataset/242) | 768 × 8 | 🟢 |
| 52 | Мониторинг состояния при Паркинсоне | Регрессия с утечкой данных | [Parkinsons Telemonitoring, UCI id=189](https://archive.ics.uci.edu/dataset/189) | 5 875 × 19 | 🟡 |
| 53 | Оценка стоимости жилья | Регрессия | [Real Estate Valuation, UCI id=477](https://archive.ics.uci.edu/dataset/477) | 414 × 6 | 🟡 |
| 54 | Прогноз арендной ставки | Регрессия, текстовые признаки | [Apartment for Rent Classified, UCI id=555](https://archive.ics.uci.edu/dataset/555) | 10 000 × 21 | 🟡 |
| 55 | Возраст морского ежа | Регрессия и классификация по группам | [Abalone, UCI id=1](https://archive.ics.uci.edu/dataset/1) | 4 177 × 8 | 🟡 |
| 56 | Качество вина | Регрессия и многоклассовая классификация | [Wine Quality, UCI id=186](https://archive.ics.uci.edu/dataset/186) | 6 497 × 11 | 🟡 |
| 57 | Прогноз мощности комбинированного цикла | Регрессия | [Combined Cycle Power Plant, UCI id=294](https://archive.ics.uci.edu/dataset/294) | 9 568 × 8 | 🟢 |
| 58 | Температура по инфракрасному снимку | Регрессия, 152 признака | [Infrared Thermography Temperature, UCI id=925](https://archive.ics.uci.edu/dataset/925) | 1 020 × 152 | 🔴 |


| № | Тема | Тип задачи | Набор данных | Объём | Уровень |
|---|---|---|---|---|---|
| 59 | Прогноз аэродинамического шума крыла | Регрессия | [Airfoil Self-Noise, UCI id=291](https://archive.ics.uci.edu/dataset/291) | 1 503 × 6 | 🟢 |
| 60 | Прогноз уровня преступности в общине | Регрессия, 127 признаков | [Communities and Crime, UCI id=183](https://archive.ics.uci.edu/dataset/183) | 1 994 × 127 | 🔴 |
| 61 | Предсказание радиационных вспышек на Солнце | Бинарная классификация, дисбаланс 20:1 | [Solar Flare, UCI id=89](https://archive.ics.uci.edu/dataset/89) | 1 389 × 3 | 🟢 |
| 62 | Предиктивное обслуживание промышленного оборудования | Бинарная классификация, дисбаланс 3.4 % | [AI4I 2020 Predictive Maintenance, UCI id=601](https://archive.ics.uci.edu/dataset/601) | 10 000 × 14 | 🟡 |
| 63 | Прогноз выбросов газовой турбины | Многомерная регрессия | [Gas Turbine CO and NOx Emission Data Set, UCI id=551](https://archive.ics.uci.edu/dataset/551) | 36 733 × 10 | 🔴 |
| 64 | Многомерная регрессия метрик социальных сетей | Многомерная регрессия | [Facebook Metrics, UCI id=368](https://archive.ics.uci.edu/dataset/368) | 500 × 18 | 🟡 |
| 65 | Предсказание энергопотребления зданий | Многомерная регрессия | [Energy Efficiency, UCI id=242](https://archive.ics.uci.edu/dataset/242) | 768 × 8 | 🟢 |
| 66 | Прогноз концентрации загрязняющих веществ в воздухе | Регрессия временного ряда | [Air Quality, UCI id=360](https://archive.ics.uci.edu/dataset/360) | 9 358 часовых | 🔴 |

## Группа 3. Кластеризация

| № | Тема | Тип задачи | Набор данных | Объём | Уровень |
|---|---|---|---|---|---|
| 67 | Сегментация клиентов интернет-магазина | Кластеризация, RFM-анализ | [Online Retail, UCI id=352](https://archive.ics.uci.edu/dataset/352) | 541 909 транзакций | 🔴 |
| 68 | Сегментация пациентов по белковому профилю | Кластеризация и классификация | [Mice Protein Expression, UCI id=342](https://archive.ics.uci.edu/dataset/342) | 1 080 × 80 | 🔴 |
| 69 | Сегментация населения США (перепись 1990) | Кластеризация больших данных | [US Census Data (1990), UCI id=116](https://archive.ics.uci.edu/dataset/116) | 2 458 285 × 68 | 🔴 |
| 70 | Сегментация объектов по профилю отзывов | Кластеризация и многозначная классификация | [Travel Review Ratings, UCI id=485](https://archive.ics.uci.edu/dataset/485) | 5 456 × 24 | 🟡 |
| 71 | Типы поведения продавцов в соцсетях | Кластеризация | [Facebook Live Sellers in Thailand, UCI id=488](https://archive.ics.uci.edu/dataset/488) | 7 051 × 11 | 🟡 |
| 72 | Химический состав стекла | Кластеризация и многоклассовая классификация | [Glass Identification, UCI id=42](https://archive.ics.uci.edu/dataset/42) | 214 × 9 | 🟢 |
| 73 | Группировка сортов сои по признакам | Кластеризация | [Forty Soybean Cultivars, UCI id=913](https://archive.ics.uci.edu/dataset/913) | 320 × 47 | 🟡 |

## Группа 4. Прогнозирование временных рядов

| № | Тема | Тип задачи | Набор данных | Объём | Уровень |
|---|---|---|---|---|---|
| 74 | Число аренд велосипедов в Вашингтоне | Временной ряд с внешними признаками | [Bike Sharing, UCI id=275](https://archive.ics.uci.edu/dataset/275) | 17 379 часовых | 🟡 |
| 75 | Спрос на велосипеды в Сеуле | Временной ряд, погодные факторы | [Seoul Bike Sharing Demand, UCI id=560](https://archive.ics.uci.edu/dataset/560) | 8 760 часовых | 🟡 |
| 76 | Концентрация бензола в воздухе | Регрессия временного ряда | [Air Quality, UCI id=360](https://archive.ics.uci.edu/dataset/360) | 9 358 часовых | 🔴 |
| 77 | Потребление энергии зданием | Регрессия и прогнозирование | [Appliances Energy Prediction, UCI id=374](https://archive.ics.uci.edu/dataset/374) | 19 735 (10 мин) | 🔴 |
| 78 | Курс акций на Стамбульской бирже | Регрессия и классификация ряда | [ISTANBUL STOCK EXCHANGE, UCI id=247](https://archive.ics.uci.edu/dataset/247) | 536 дневных | 🔴 |
| 79 | Бытовые показания электросчётчика | Прогнозирование и поиск аномалий | [Individual Household Electric Power Consumption, UCI id=235](https://archive.ics.uci.edu/dataset/235) | 2 075 259 (1 мин) | 🔴 |
| 80 | Прогноз потребления электроэнергии в городе | Регрессия временного ряда | [Power Consumption of Tetouan City, UCI id=849](https://archive.ics.uci.edu/dataset/849) | 52 417 часовых наблюдений | 🔴 |


| № | Тема | Тип задачи | Набор данных | Объём | Уровень |
|---|---|---|---|---|---|
| 81 | Прогноз концентрации PM2.5 в воздухе | Регрессия временного ряда | [Beijing PM2.5 Data, UCI id=381](https://archive.ics.uci.edu/dataset/381) | 43 824 почасовых | 🔴 |
| 82 | Прогноз популярности интернет-новостей | Регрессия | [Online News Popularity, UCI id=332](https://archive.ics.uci.edu/dataset/332) | 39 797 × 58 | 🔴 |
| 83 | Формирование инвестиционного портфеля | Регрессия, 63 целевые переменные | [Stock Portfolio Performance, UCI id=390](https://archive.ics.uci.edu/dataset/390) | 315 × 6 | 🔴 |
| 84 | Прогноз суточного спроса на товары | Регрессия временного ряда | [Daily Demand Forecasting Orders, UCI id=409](https://archive.ics.uci.edu/dataset/409) | 60 суток × 13 | 🟡 |
| 85 | Прогноз энергопотребления бытовых приборов | Регрессия | [Appliances Energy Prediction, UCI id=374](https://archive.ics.uci.edu/dataset/374) | 19 735 (10 мин) | 🔴 |

## Группа 5. Текст и анализ тональности

| № | Тема | Тип задачи | Набор данных | Объём | Уровень |
|---|---|---|---|---|---|
| 86 | Спам в комментариях YouTube | Классификация короткого текста | [YouTube Spam Collection, UCI id=380](https://archive.ics.uci.edu/dataset/380) | 1 956 комментариев | 🟡 |

## Группа 6. Специальные задачи

| № | Тема | Тип задачи | Набор данных | Объём | Уровень |
|---|---|---|---|---|---|
| 87 | Рекомендательная система товаров | Коллаборативная фильтрация, матричная факторизация | [Online Retail, UCI id=352](https://archive.ics.uci.edu/dataset/352) | 4 338 клиентов × 4 093 товара | 🔴 |
| 88 | Выживаемость после инфаркта | Анализ выживаемости (survival analysis) | [Echocardiogram, UCI id=38](https://archive.ics.uci.edu/dataset/38) | 132 пациента × 9 | 🔴 |

## Группа 7. Кластеризация и снижение размерности

| № | Тема | Тип задачи | Набор данных | Объём | Уровень |
|---|---|---|---|---|---|
| 89 | Сегментация оптовых клиентов | Кластеризация | [Wholesale customers, UCI id=292](https://archive.ics.uci.edu/dataset/292) | 440 × 6 | 🟢 |
| 90 | Выявление сезонных паттернов продаж | Кластеризация временных рядов | [Sales Transactions Weekly, UCI id=396](https://archive.ics.uci.edu/dataset/396) | 811 недель × 10 | 🟡 |
| 91 | Анализ динамики фондового индекса | Кластеризация временных рядов | [Dow Jones Index, UCI id=312](https://archive.ics.uci.edu/dataset/312) | 750 месяцев × 30 | 🟡 |
| 92 | Типизация страниц веб-сайта по назначению | Кластеризация и классификация | [Page Blocks Classification, UCI id=78](https://archive.ics.uci.edu/dataset/78) | 5 473 × 10 | 🟡 |
| 93 | Предсказание пола по имени | Бинарная классификация текста и кластеризация | [Gender by Name, UCI id=591](https://archive.ics.uci.edu/dataset/591) | 147 270 имён | 🔴 |

## Группа 8. Компьютерное зрение по векторам признаков

| № | Тема | Тип задачи | Набор данных | Объём | Уровень |
|---|---|---|---|---|---|
| 94 | Распознавание цифр по траектории письма | Многоклассовая классификация | [Pen-Based Recognition of Handwritten Digits, UCI id=81](https://archive.ics.uci.edu/dataset/81) | 10 992 × 16 | 🟡 |
| 95 | Классификация силуэтов транспортных средств | Многоклассовая классификация изображений | [Statlog (Vehicle Silhouettes), UCI id=149](https://archive.ics.uci.edu/dataset/149) | 946 силуэтов × 18 | 🟡 |
| 96 | Распознавание букв по акустической сигнатуре | Многоклассовая классификация (26 классов) | [ISOLET, UCI id=54](https://archive.ics.uci.edu/dataset/54) | 7 797 × 617 | 🔴 |

## Группа 9. Специальные задачи и структурированные данные

| № | Тема | Тип задачи | Набор данных | Объём | Уровень |
|---|---|---|---|---|---|
| 97 | Классификация интронов по последовательностям нуклеотидов | Классификация структурированных последовательностей | [Molecular Biology (Splice-junction Gene Sequences), UCI id=69](https://archive.ics.uci.edu/dataset/69) | 3 190 × 60 | 🔴 |
| 98 | Прогноз уровня озона | Классификация, дисбаланс 4 % | [Ozone Level Detection, UCI id=172](https://archive.ics.uci.edu/dataset/172) | 2 536 суток × 72 | 🔴 |
| 99 | Определение победителя в игре «Connect-4» | Многоклассовая классификация (3 класса) | [Connect-4, UCI id=26](https://archive.ics.uci.edu/dataset/26) | 67 557 позиций × 42 | 🟡 |
| 100 | Эндшпиль в шахматах: оценка позиции по 6 признакам | Многоклассовая классификация (12 классов) | [Chess (King-Rook vs. King), UCI id=23](https://archive.ics.uci.edu/dataset/23) | 28 056 позиций × 6 | 🟡 |
