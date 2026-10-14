[![en](https://img.shields.io/badge/lang-en-blue.svg)](README.md)

# Дмитрий Кобелев

Количественный аналитик, переходящий в **AI governance, валидацию моделей и оценку LLM**.
Бэкграунд: радиофизика (МГУ им. Ломоносова), более 12 лет в телекоме, где отвечал за прогнозы выручки, на которые опиралось высшее руководство, и прикладной data science с 2023 года.

Я проверяю, как LLM-системы принятия решений ведут себя на самом деле: не только верен ли ответ, но и устойчиво ли решение, чувствительно ли оно к нужным свидетельствам, честно ли названы причины и понимает ли модель, когда нужно задать вопрос, а не отвечать.

[LinkedIn](https://www.linkedin.com/in/dima-does-code) · [Hugging Face](https://huggingface.co/dima-does-code)

---

## Валидация LLM-решений

Серия небольших воспроизводимых black-box экспериментов на синтетических данных. Общий метод: контролируемые кейсы и парные возмущения, эталонные решения заданы заранее, сырые ответы сохраняются, типы отказов названы, ограничения указаны сразу.

| Проект | Вопрос | Главный результат |
|---|---|---|
| [LLM-Financial-Validation](https://github.com/DimaDoesCode/LLM-Financial-Validation) | Зависит ли финансовое решение LLM от формулировки, подачи и обсуждения случая? | 86% точности в целом, но около 50% на кейсах с противоречивыми сигналами; прослеживаемость обоснований слабая (15,8% в целом) |
| [LLM-Style-Audit](https://github.com/DimaDoesCode/LLM-Style-Audit) | Вознаграждает ли LLM то, как вы пишете, а не то, что говорите? | При явной политике 0 из 120 сравнений стиля изменили решение; при дискреции рецензента все 9 изменений из-за стиля пошли в сторону APPROVE |
| [LLM-Evidence-Update-Validation](https://github.com/DimaDoesCode/LLM-Evidence-Update-Validation) | Пересматривает ли модель решение в нужный момент, когда свидетельства приходят по шагам? | 100% точности финального решения, но только 60% полностью верных траекторий |
| [LLM-Validation-Should-the-LLM-Ask](https://github.com/DimaDoesCode/LLM-Validation-Should-the-LLM-Ask) | Знает ли модель, когда отвечать, когда спросить, а когда оспорить ложную посылку? | 78,6% в целом; 50% на существенно неоднозначных запросах и на ложных посылках |
| [LLM-Validation-Candidate-Screening-Ranking-Stability](https://github.com/DimaDoesCode/LLM-Validation-Candidate-Screening-Ranking-Stability) | Стабильно ли и чувствительно ли к свидетельствам ранжирование кандидатов LLM? | 40/40 верно, это эффект потолка, а не доказательство; V2 строится вокруг близких кандидатов и повторных прогонов |

**Общие ограничения.** Синтетические данные, одна модель (`openai/gpt-oss-120b` через Groq), temperature 0, малые выборки. Это прототипы валидации и демонстрация метода, а не бенчмарки и не свидетельство о реальных системах. Дальше для всей серии: повторные прогоны, вторая модель и доверительные интервалы для каждой метрики.

---

## Другие проекты

**[MAC-Shaper](https://github.com/DimaDoesCode/MAC-Shaper)**: ограничение входящей и исходящей полосы по MAC-адресам для OpenWrt (Linux `tc` и `ifb`), со скриптом, веб-интерфейсом LuCI и готовыми пакетами.

**[HA-OpenWrt-SSH](https://github.com/DimaDoesCode/HA-OpenWrt-SSH)**: интеграция Home Assistant для мониторинга роутеров OpenWrt по SSH (температура CPU, нагрузка, RAM, статус VPN, диск). Готова для HACS.

**Hybrid Conversation** (Home Assistant + Ollama): интеграция, которая направляет каждый запрос либо в детерминированный движок интентов, либо в локальную LLM. <!-- TODO: добавить ссылку на репозиторий -->

### Прикладной ML и NLP

| Проект | Описание |
|---|---|
| [NPD prediction](https://github.com/DimaDoesCode/ML_and_Time-Series) | Предсказание даты следующей покупки (классический ML) |
| [NP Multilabel prediction](https://github.com/DimaDoesCode/ML_DL_Multilabel_Prediction) | Следующий заказ как набор категорий товаров (нейросеть) |
| [DL & NLP: GeoNames](https://github.com/DimaDoesCode/DL_and_NLP-Geonames) | Нормализация географических названий по GeoNames |
| [DL & CV: Music Genre Prediction](https://github.com/DimaDoesCode/VC_Predicting_Music_Genre) | Классификация жанра музыки по обложкам альбомов |

<details>
<summary>Яндекс Практикум: проекты программы Data Science (2023)</summary>

| Проект | Тема |
|---|---|
| [Basic Python](https://github.com/DimaDoesCode/Yandex_Practicum-Big_City_Music) | Проверка данных и сравнение поведения пользователей на данных Яндекс.Музыки |
| [Data preprocessing](https://github.com/DimaDoesCode/Yandex_Practicum-Borrower_Reliability_Study) | Влияние семейного положения и детей на возврат кредита |
| [Exploratory Data Analysis](https://github.com/DimaDoesCode/Yandex_Practicum-Exploratory_Data_Analysis) | Анализ рынка недвижимости |
| [Statistical Data Analysis](https://github.com/DimaDoesCode/Yandex_Practicum-Statistical_Data_analysis) | Анализ поведения клиентов для оптимизации тарифов |
| [Composite Project 1](https://github.com/DimaDoesCode/Yandex_Practicum-Composite_Project-1) | Закономерности, определяющие успех игр |
| [Introduction to Machine Learning](https://github.com/DimaDoesCode/Yandex_Practicum-Introduction_to_Machine_Learning) | Модель классификации для выбора тарифа |
| [Supervised Learning](https://github.com/DimaDoesCode/Yandex_Practicum-Supervised_Learning) | Предсказание оттока клиентов банка |
| [Machine Learning in Business](https://github.com/DimaDoesCode/Yandex_Practicum-Machine_Learning_in_Business) | Анализ прибыли и рисков для регионов нефтедобычи |
| [Composite Project 2](https://github.com/DimaDoesCode/Yandex_Practicum-Composite_Project-2) | Предсказание коэффициента извлечения золота в промышленном процессе |
| [Linear Algebra](https://github.com/DimaDoesCode/Yandex_Practicum-Linear_Algebra) | Преобразование данных для защиты персональной информации |
| [Numerical Analysis](https://github.com/DimaDoesCode/Yandex_Practicum-Numerical_Analysis) | Предсказание цены автомобиля |
| [Time Series](https://github.com/DimaDoesCode/Yandex_Practicum-Time_Series) | Прогноз спроса на такси в аэропортах |
| [Machine Learning for Text](https://github.com/DimaDoesCode/Yandex_Practicum-Machine_Learning_for_Text) | Выявление токсичных комментариев |
| [Computer Vision](https://github.com/DimaDoesCode/Yandex_Practicum-Computer_Vision) | Предсказание возраста по фотографии лица |
| [Diploma Project](https://github.com/DimaDoesCode/Yandex_Practicum-Diploma_Project) | Предсказание оттока клиентов телеком-оператора |

</details>

---

Большинство проектов здесь это самостоятельная работа, продиктованная техническим любопытством и желанием понять системы и со стороны данных, и со стороны низкоуровневой инженерии.
