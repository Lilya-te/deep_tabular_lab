# Deep Tabular Lab

Проект для анализа LMS-логов и построения модели прогнозирования оттока студентов.

## Структура проекта

```text
deep_tabular_lab/
├── README.md
├── .gitignore
├── docs/
│   ├── task.md
│   ├── task_new.md
│   ├── tables_description.pdf
│   ├── Transfer criteria.pdf
│   └── tables_description_new.pdf
├── notebooks/
│   ├── requirements.txt
│   ├── 01_eda_and_features.ipynb
│   ├── 02_dropout_prediction_model.ipynb
│   ├── 03_eda_hypothesis.ipynb
│   └── 04_final_v1.ipynb
└── presentation/
```

Локальные каталоги (не коммитятся, см. `.gitignore`): `.venv/`, `notebooks/tmp/`, `.cursor/`.

## Описание каталогов

- `docs/` — постановка задачи, описание таблиц и критериев (markdown и PDF).
- `docs/task.md` — формализованное условие проектной задачи.
- `docs/task_new.md` — актуализированная формулировка задачи (при наличии).
- `docs/tables_description.pdf` и `docs/tables_description_new.pdf` — описание таблиц датасета.
- `notebooks/` — основной пайплайн в Jupyter Notebook; зависимости перечислены в `notebooks/requirements.txt`.
- `notebooks/01_eda_and_features.ipynb` — EDA, очистка таблиц, признаки, маски и сбор таргета.
- `notebooks/02_dropout_prediction_model.ipynb` — обучение, оценка и интерпретация модели оттока.
- `notebooks/03_eda_hypothesis.ipynb` — проверка гипотез и дополнительный EDA.
- `notebooks/04_final_v1.ipynb` — финальный прогон пайплайна (версия v1).
- `presentation/` — материалы презентации решения (каталог-заглушка в репозитории).


### `01_eda_and_features.ipynb`
Базовый EDA-ноутбук: очистка таблиц, формирование признаков, построение критериев и сбор таргета для обучения.

### `02_dropout_prediction_model.ipynb`
Ноутбук с baseline-моделью прогнозирования оттока: обучение, валидация качества и интерпретация результатов.

### `03_eda_hypothesis.ipynb`
Исследовательский ноутбук для проверки отдельных гипотез на подготовленных данных.

### `04_final_v1.ipynb`
Финальная интегрированная версия пайплайна с этапами анализа, очистки и подготовки данных к моделированию.

## Хранение данных
[исходные датасеты, предоставленные заказчиком](https://drive.google.com/drive/folders/1aoMxqBCuux2i9jBTjEmmopVfOYzYOgR-?usp=sharing) 
[сформированные датасеты для исследования и построения модели](https://drive.google.com/drive/folders/1pf7F__1ZCMtMGbjkGr1NsLss7vO7zkOk?usp=sharing) 