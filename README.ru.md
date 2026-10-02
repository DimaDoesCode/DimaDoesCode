[![en](https://img.shields.io/badge/lang-en-blue.svg)](https://github.com/DimaDoesCode/DimaDoesCode/blob/master/README.md)

# Аудит решений AI | Валидация LLM и AI-систем

Я занимаюсь **валидацией и аудитом систем принятия решений на основе AI**, с особым фокусом на Large Language Models (LLM).

В текущей работе меня интересует поведение AI-систем при принятии решений — не только правильность ответа, но и то, сохраняется ли решение **последовательным, устойчивым, воспроизводимым и объяснимым при изменении контекста взаимодействия**.

Основные направления:

- **Валидация решений LLM**
- **AI / Model Risk**
- **Корректность и согласованность решений**
- **Тестирование устойчивости и стабильности**
- **Чувствительность к формулировке контекста (framing sensitivity)**
- **Риски взаимодействия человека и LLM**
- **Трассируемость решений**
- **Воспроизводимые validation-процессы на Python**

Мой профессиональный опыт объединяет **физику, разработку ПО, телекоммуникации, бизнес-аналитику и Data Science**.

Большинство проектов в этом профиле — **независимые и pet-проекты**, созданные для исследования практических технических задач, а не как коммерческая разработка для крупных организаций.

---

## Валидация и аудит LLM

Проекты, посвящённые **валидации и аудиту решений систем на основе LLM** — не просто разработке с использованием LLM, а проверке того, насколько их решения корректны, последовательны и справедливы при внимательном рассмотрении.

### [LLM Financial Decision Validation](https://github.com/DimaDoesCode/LLM-Financial-Validation)

Компактный фреймворк для валидации **финансовой системы принятия решений на основе LLM**.

**Human ↔ LLM ↔ Decision**

Фреймворк выходит за рамки обычной оценки accuracy и исследует поведение системы по нескольким направлениям:

- Корректность решений
- Согласованность и стабильность
- Чувствительность к формулировке контекста
- Отражение позиции пользователя
- Закрепление пользовательских убеждений
- Трассируемость решений

*Portfolio project · MIT License*

### [LLM Style Audit](https://github.com/DimaDoesCode/LLM-Style-Audit)

Вознаграждает ли LLM за *то, как* написан текст, а не за *то, что* в нём сказано? Аудит решений LLM на синтетических заявках на социальные льготы, где одни и те же факты поданы в разных стилях — формальном, небрежно-грубом, эмоциональном и на русском языке.

Три проверки: точность по стилям относительно эталона, вычисленного кодом; *цена стиля* — сдвиг доли одобрений относительно формального базового варианта; и раскрывает ли модель влияние стиля в своём обосновании, когда решение меняется.

*Portfolio project · MIT License*

### [LLM Evidence Update Validation](https://github.com/DimaDoesCode/LLM-Evidence-Update-Validation)

Способна ли LLM пересмотреть решение, когда новые данные требуют разворота — и при этом сохранять стабильность, когда разворот не требуется? Эксперимент на последовательном поступлении улик с синтетическими кейсами диагностики инцидентов, опирающийся на исследования belief revision и anchoring-эффектов.

Разделяет **точность финального решения** и **корректность траектории решения**: в V1 финальная точность составила 100%, но полностью корректную траекторию модель прошла лишь в 60% случаев — то есть решение иногда меняется на шаг раньше или позже, даже если итоговый ответ верный.

*Portfolio project · MIT License*

---

## Избранные проекты

### [Northstar Model Validation](https://github.com/DimaDoesCode/Northstar-Model-Validation)

Независимый **фреймворк Model Risk и Model Validation** для ML-модели кредитного риска.

Охватывает discrimination, calibration, stability и segment performance, разделяя **характеристики модели, validation evidence и итоговые validation conclusions**.

*Portfolio project · MIT License*

### [MAC-Shaper](https://github.com/DimaDoesCode/MAC-Shaper)

Лёгкое решение для **управления сетевым трафиком в OpenWrt**, обеспечивающее ограничение скорости загрузки и выгрузки для отдельных MAC-адресов с использованием Linux `tc` и `ifb`.

Включает backend, интерфейс LuCI и пакеты для embedded-устройств.

*Independent systems / networking project*

---

## Home Assistant & Local AI

### [HA-OpenWrt-SSH](https://github.com/DimaDoesCode/HA-OpenWrt-SSH)

Custom integration для Home Assistant, обеспечивающая мониторинг роутеров OpenWrt через SSH.

Предоставляет данные о температуре CPU, нагрузке, RAM, VPN и дисковом пространстве.

### [HA-Hybrid-Conversation](https://github.com/DimaDoesCode/HA-Hybrid-Conversation)

Custom integration для Home Assistant, объединяющая штатный conversation agent с **локальной LLM Ollama** для формирования свободных ответов.

*No cloud API required · MIT License*

---

## Технический опыт

До перехода в Data Science и AI validation моя работа включала:

- Разработку ПО и системную интеграцию
- Телекоммуникационные и сетевые системы
- Linux / Unix
- Техническую поддержку и IT-инфраструктуру
- Бизнес-аналитику и прогнозирование выручки
- Математическое моделирование

Этот опыт продолжает определять мой подход к AI-системам: **я рассматриваю их как системы, которые необходимо тестировать, измерять и понимать, а не только как модели, которые нужно обучать.**

---

## Data Science & Machine Learning — Portfolio

### Classical ML

| Проект | Задача | Статус |
|:-------|:-------|:-------|
| [NPD prediction](https://github.com/DimaDoesCode/ML_and_Time-Series) | Предсказание следующей покупки для анализа поведения клиентов и оптимизации бизнес-решений. | Complete |
| [NP Multilabel prediction](https://github.com/DimaDoesCode/ML_DL_Multilabel_Prediction) | Предсказание следующего заказа пользователя как набора категорий товаров с использованием полносвязной нейронной сети. | Complete |

<br>

### Yandex Data Science Practicum

| Проект | Задача | Статус |
|:-------|:-------|:-------|
| [Basic Python](https://github.com/DimaDoesCode/Yandex_Practicum-Big_City_Music) | Проверка данных и сравнение поведения пользователей на реальных данных Yandex.Music. | Complete |
| [Data preprocessing](https://github.com/DimaDoesCode/Yandex_Practicum-Borrower_Reliability_Study) | Исследование влияния семейного положения и наличия детей на возврат кредита. | Complete |
| [Exploratory Data Analysis](https://github.com/DimaDoesCode/Yandex_Practicum-Exploratory_Data_Analysis) | Анализ рынка недвижимости на данных Yandex.Real Estate. | Complete |
| [Statistical Data Analysis](https://github.com/DimaDoesCode/Yandex_Practicum-Statistical_Data_analysis) | Анализ поведения клиентов для оптимизации тарифов. | Complete |
| [Composite Project - 1](https://github.com/DimaDoesCode/Yandex_Practicum-Composite_Project-1) | Выявление закономерностей, определяющих успешность компьютерных игр. | Complete |
| [Introduction to Machine Learning](https://github.com/DimaDoesCode/Yandex_Practicum-Introduction_to_Machine_Learning) | Построение модели классификации для выбора тарифа. | Complete |
| [Supervised Learning](https://github.com/DimaDoesCode/Yandex_Practicum-Supervised_Learning) | Предсказание оттока клиентов банка. | Complete |
| [Machine Learning in Business](https://github.com/DimaDoesCode/Yandex_Practicum-Machine_Learning_in_Business) | Анализ прибыли и рисков для регионов добычи нефти. | Complete |
| [Composite Project - 2](https://github.com/DimaDoesCode/Yandex_Practicum-Composite_Project-2) | Предсказание коэффициента восстановления золота в промышленном процессе. | Complete |
| [Linear Algebra](https://github.com/DimaDoesCode/Yandex_Practicum-Linear_Algebra) | Преобразование данных для защиты персональной информации. | Complete |
| [Numerical Analysis](https://github.com/DimaDoesCode/Yandex_Practicum-Numerical_Analysis) | Предсказание стоимости автомобилей по техническим характеристикам. | Complete |
| [Time Series](https://github.com/DimaDoesCode/Yandex_Practicum-Time_Series) | Прогнозирование спроса на такси в аэропортах. | Complete |
| [Machine Learning for Text](https://github.com/DimaDoesCode/Yandex_Practicum-Machine_Learning_for_Text) | Определение токсичных комментариев для модерации. | Complete |
| [Computer Vision](https://github.com/DimaDoesCode/Yandex_Practicum-Computer_Vision) | Предсказание возраста по фотографии. | Complete |
| [Diploma Project](https://github.com/DimaDoesCode/Yandex_Practicum-Diploma_Project) | Предсказание оттока клиентов телекоммуникационного оператора. | Complete |

<br>

### Deep Learning: NLP & Computer Vision

| Проект | Задача | Статус |
|:-------|:-------|:-------|
| [DL & NLP – GeoNames](https://github.com/DimaDoesCode/DL_and_NLP-Geonames) | Нормализация географических названий с использованием GeoNames. | Complete |
| [DL & CV – Music Genre Prediction](https://github.com/DimaDoesCode/VC_Predicting_Music_Genre) | Классификация музыкального жанра по изображению обложки альбома. | Complete |

<br>

---

<img src="https://komarev.com/ghpvc/?username=DimaDoesCode&style=flat-square&color=blue" alt=""/>