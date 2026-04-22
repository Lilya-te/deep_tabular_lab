# Deep Tabular Lab

Проект для анализа LMS-логов и построения модели прогнозирования оттока студентов.

## Структура проекта

```text
deep_tabular_lab/
├── README.md
├── .gitignore
├── lgb_full_checkpoint.pkl
├── scored_sample/
│   └── predictions_m3_m4.csv
├── docs/
│   ├── task.md
│   └── task_new.md
├── notebooks/
│   ├── requirements.txt
│   ├── 01_eda_and_features.ipynb
│   ├── 02_dropout_prediction_model.ipynb
│   ├── 03_final_v1.ipynb
│   └── 03_final_v2.ipynb
└── presentation/
    └── conclusions.md
```

Локальные каталоги (не коммитятся, см. `.gitignore`): `.venv/`, `notebooks/tmp/`, `.cursor/`.

## Описание каталогов

- `docs/` — постановка задачи и ее уточненная версия.
- `docs/task.md` — формализованное условие проектной задачи.
- `docs/task_new.md` — актуализированная формулировка задачи (при наличии).
- `notebooks/` — основной пайплайн в Jupyter Notebook; зависимости перечислены в `notebooks/requirements.txt`.
- `notebooks/01_eda_and_features.ipynb` — EDA, очистка таблиц, формирование критериев, таргета и признаков.
- `notebooks/02_dropout_prediction_model.ipynb` — baseline-модель оттока, валидация и интерпретация признаков.
- `notebooks/03_final_v1.ipynb` — первая интегрированная версия финального пайплайна.
- `notebooks/03_final_v2.ipynb` — **актуальная** финальная версия с проверкой утечек и априорной моделью.
- `lgb_full_checkpoint.pkl` — сохраненный checkpoint обученной модели LightGBM для повторного использования без переобучения.
- `scored_sample/` — примеры результатов скоринга модели.
- `scored_sample/predictions_m3_m4.csv` — прогнозы для студентов модулей M3/M4 (вероятности и уровни риска).
- `presentation/` — материалы итоговой презентации.
- `presentation/conclusions.md` — структурированные выводы и бизнес-рекомендации по результатам анализа.


### `01_eda_and_features.ipynb`
Базовый EDA-ноутбук: очистка таблиц, построение критериев, сбор целевой переменной и формирование признаков с применением маски ранних данных.

### `02_dropout_prediction_model.ipynb`
Ноутбук с baseline-моделью прогнозирования оттока: обучение, валидация качества и интерпретация результатов.

### `03_final_v1.ipynb`
Финальная интегрированная версия пайплайна с этапами анализа, очистки и подготовки данных к моделированию.

### `03_final_v2.ipynb`
Актуальная версия финального ноутбука: переопределение постановки задачи на уровне студента, фильтрация утечек, обучение на "честных" априорных признаках и прогнозы для M3/M4.

## Хранение данных

- [Исходные датасеты, предоставленные заказчиком](https://drive.google.com/drive/folders/1aoMxqBCuux2i9jBTjEmmopVfOYzYOgR-?usp=sharing)
- [Сформированные датасеты для исследования и построения модели](https://drive.google.com/drive/folders/1pf7F__1ZCMtMGbjkGr1NsLss7vO7zkOk?usp=sharing)