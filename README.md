# Deep Tabular Lab

Проект для анализа LMS-логов и построения модели прогнозирования оттока студентов.

Правила работы с репозиторием:
- в ветке main храним ноутбук с очищенными ячейками и сброшенным ядром для того чтобы было удобно мержиться
- пуш в main закрыт, отправить код в main ветку можно только через пул реквест

## Структура проекта

```text
deep_tabular_lab/
├── README.md
├── .gitignore
├── docs/
│   └── task.md
├── notebooks/
│   ├── 01_eda_and_features.ipynb
│   └── 02_dropout_prediction_model.ipynb
├── data/
│   ├── interim/
│   └── processed/
├── artifacts/
│   ├── models/
│   ├── reports/
│   └── figures/
└── presentation/
```

## Описание каталогов

- `docs/` — материалы постановки задачи и сопроводительная документация.
- `docs/task.md` — формализованное условие проектной задачи.
- `notebooks/` — основной пайплайн решения в Jupyter Notebook.
- `notebooks/01_eda_and_features.ipynb` — EDA, первичный анализ и построение признаков.
- `notebooks/02_dropout_prediction_model.ipynb` — обучение, оценка и интерпретация модели.
- `data/interim/` — промежуточные наборы после очистки и объединений.
- `data/processed/` — финальные датасеты для моделирования.
- `artifacts/models/` — сохраненные модели и веса.
- `artifacts/reports/` — аналитические отчеты и текстовые результаты.
- `artifacts/figures/` — графики и визуализации.
- `presentation/` — финальная презентация решения.



