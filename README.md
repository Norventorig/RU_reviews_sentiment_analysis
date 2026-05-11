# Russian NLP Sentiment Classification

Классификация тональности русскоязычных текстов с использованием классических ML-подходов и Transformer-моделей.

---

# О проекте

Цель проекта — автоматизировать анализ пользовательских текстов и определить их эмоциональную окраску (sentiment classification).

В рамках проекта были реализованы и сравнены:

* классический ML pipeline:

  * TF-IDF
  * Logistic Regression

* современные Transformer-модели:

  * RuBERT
  * DeBERTa

Проект включает:

* анализ данных (EDA)
* предобработку текста
* обучение моделей
* сравнение метрик
* визуализацию результатов

---

# Используемые данные

Датасет содержит русскоязычные тексты с метками тональности.

Примеры классов:

* positive
* neutral
* negative

---

# Exploratory Data Analysis (EDA)

В рамках анализа данных были исследованы:

* распределение классов
* длина текстов
* дисбаланс классов
* статистика текстов

Также была проведена:

* очистка текста
* токенизация
* подготовка данных для Transformer-моделей

---

# Используемые технологии

Основные библиотеки:

* Python
* Pandas
* NumPy
* Scikit-learn
* PyTorch
* Transformers
* Matplotlib
* Seaborn

---

# Модели

## TF-IDF + Logistic Regression

Базовый ML pipeline:

* TF-IDF vectorization
* Logistic Regression classifier

Использовался как baseline для сравнения с Transformer-моделями.

---

## RuBERT

Русскоязычная Transformer-модель на основе BERT.

Использовалась для:

* contextual embeddings
* классификации текстов

---

## DeBERTa

Более современная Transformer-архитектура с улучшенным механизмом attention.

---

# Метрики

Для оценки качества моделей использовались:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC

---

# Результаты

| Model                        | Accuracy | F1-score |
| ---------------------------- | -------- | -------- |
| TF-IDF + Logistic Regression | 0.65     | 0.65     |
| RuBERT                       | 0.70     | 0.70     |
| DeBERTa                      | 0.72     | 0/72     |

---

# Основные выводы

* Transformer-модели показали более высокое качество по сравнению с baseline.
* TF-IDF + Logistic Regression обеспечивает хорошее качество при низких вычислительных затратах.
* Предобработка и балансировка классов существенно влияют на итоговые метрики.

---

# Возможные улучшения

* Hyperparameter tuning
* Cross-validation
* Deployment через FastAPI
* Docker контейнеризация
* MLflow для отслеживания экспериментов
* Streamlit интерфейс

---

# Автор

Гордей — Junior Data Scientist / Data Analyst

GitHub: (https://github.com/Norventorig)
