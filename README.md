[![ru](https://img.shields.io/badge/lang-ru-blue.svg)](README.ru.md)

# Dmitry Kobelev

Quantitative analyst moving into **AI governance, model validation and LLM evaluation**.
Background: Radiophysics (Lomonosov Moscow State University), 12+ years in telecom owning revenue forecasts that senior leadership relied on, and applied data science since 2023.

I test how LLM-based decision systems actually behave: not only whether the answer is correct, but whether the decision is stable, sensitive to the right evidence, honest about its reasons, and aware of when to ask instead of answer.

[LinkedIn](https://www.linkedin.com/in/dima-does-code) · [Hugging Face](https://huggingface.co/dima-does-code)

---

## LLM decision validation

A series of small, reproducible black-box experiments on synthetic data. Shared method: controlled cases and paired perturbations, reference decisions fixed in advance, raw outputs stored, failure modes named, limitations stated up front.

| Project | Question | Headline result |
|---|---|---|
| [LLM-Financial-Validation](https://github.com/DimaDoesCode/LLM-Financial-Validation) | Does an LLM financial decision depend on how the case is worded, framed and discussed? | 86% accuracy overall, but about 50% on conflicting-signal cases; rationale traceability is weak (15.8% overall) |
| [LLM-Style-Audit](https://github.com/DimaDoesCode/LLM-Style-Audit) | Does an LLM reward how you write, not what you say? | Under an explicit policy 0 of 120 style comparisons changed a decision; with reviewer discretion all 9 style-driven changes went toward APPROVE |
| [LLM-Evidence-Update-Validation](https://github.com/DimaDoesCode/LLM-Evidence-Update-Validation) | Does the model revise a decision at the right moment when evidence arrives step by step? | 100% final accuracy, but only 60% fully correct decision trajectories |
| [LLM-Validation-Should-the-LLM-Ask](https://github.com/DimaDoesCode/LLM-Validation-Should-the-LLM-Ask) | Does the model know when to answer, ask, or challenge a false premise? | 78.6% overall; 50% on materially ambiguous requests and on false premises |
| [LLM-Validation-Candidate-Screening-Ranking-Stability](https://github.com/DimaDoesCode/LLM-Validation-Candidate-Screening-Ranking-Stability) | Is an LLM ranking of job candidates stable and evidence-sensitive? | 40/40 correct, which is a ceiling effect rather than proof; V2 is designed around near-ties and repeated runs |

**Common limitations.** Synthetic data, one model (`openai/gpt-oss-120b` via Groq), temperature 0, small samples. These are validation prototypes and method demonstrations, not benchmarks and not evidence about any real system. Next steps across the series: repeated runs, a second model, and confidence intervals for every metric.

---

## Other projects

**[MAC-Shaper](https://github.com/DimaDoesCode/MAC-Shaper)**: per-MAC upload and download bandwidth control for OpenWrt (Linux `tc` and `ifb`), with a backend script, LuCI web interface and prebuilt packages.

**[HA-OpenWrt-SSH](https://github.com/DimaDoesCode/HA-OpenWrt-SSH)**: Home Assistant custom integration for OpenWrt router monitoring over SSH (CPU temperature, load, RAM, VPN status, disk usage). HACS-ready.

**Hybrid Conversation** (Home Assistant + Ollama): integration that routes each request between a deterministic rule-based intent engine and a local LLM. <!-- TODO: add repository link -->

### Applied ML and NLP

| Project | Description |
|---|---|
| [NPD prediction](https://github.com/DimaDoesCode/ML_and_Time-Series) | Next purchase date prediction (classical ML) |
| [NP Multilabel prediction](https://github.com/DimaDoesCode/ML_DL_Multilabel_Prediction) | Next order as a set of product categories (neural network) |
| [DL & NLP: GeoNames](https://github.com/DimaDoesCode/DL_and_NLP-Geonames) | Geographical name normalization against GeoNames |
| [DL & CV: Music Genre Prediction](https://github.com/DimaDoesCode/VC_Predicting_Music_Genre) | Music genre classification from album covers |

<details>
<summary>Yandex Practicum: Data Science program projects (2023)</summary>

| Project | Topic |
|---|---|
| [Basic Python](https://github.com/DimaDoesCode/Yandex_Practicum-Big_City_Music) | Data validation and user behavior comparison on Yandex.Music data |
| [Data preprocessing](https://github.com/DimaDoesCode/Yandex_Practicum-Borrower_Reliability_Study) | Impact of family status and children on loan repayment |
| [Exploratory Data Analysis](https://github.com/DimaDoesCode/Yandex_Practicum-Exploratory_Data_Analysis) | Real estate market analysis |
| [Statistical Data Analysis](https://github.com/DimaDoesCode/Yandex_Practicum-Statistical_Data_analysis) | Customer behavior analysis for tariff optimization |
| [Composite Project 1](https://github.com/DimaDoesCode/Yandex_Practicum-Composite_Project-1) | Patterns that determine game success |
| [Introduction to Machine Learning](https://github.com/DimaDoesCode/Yandex_Practicum-Introduction_to_Machine_Learning) | Classification model for tariff selection |
| [Supervised Learning](https://github.com/DimaDoesCode/Yandex_Practicum-Supervised_Learning) | Bank customer churn prediction |
| [Machine Learning in Business](https://github.com/DimaDoesCode/Yandex_Practicum-Machine_Learning_in_Business) | Profit and risk analysis for oil extraction regions |
| [Composite Project 2](https://github.com/DimaDoesCode/Yandex_Practicum-Composite_Project-2) | Gold recovery rate prediction in industrial processes |
| [Linear Algebra](https://github.com/DimaDoesCode/Yandex_Practicum-Linear_Algebra) | Data transformation for personal information protection |
| [Numerical Analysis](https://github.com/DimaDoesCode/Yandex_Practicum-Numerical_Analysis) | Car price prediction |
| [Time Series](https://github.com/DimaDoesCode/Yandex_Practicum-Time_Series) | Taxi demand forecasting at airports |
| [Machine Learning for Text](https://github.com/DimaDoesCode/Yandex_Practicum-Machine_Learning_for_Text) | Toxic comment detection |
| [Computer Vision](https://github.com/DimaDoesCode/Yandex_Practicum-Computer_Vision) | Age prediction from facial images |
| [Diploma Project](https://github.com/DimaDoesCode/Yandex_Practicum-Diploma_Project) | Customer churn prediction for a telecom operator |

</details>

---

Most projects here are independent work driven by technical curiosity and a wish to understand systems both from the data side and from the low-level engineering side.
