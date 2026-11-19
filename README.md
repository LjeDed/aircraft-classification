# aircraft-classification

# Классификация самолётов с помощью Vision-Language Models

Сравнение мультимодальных моделей для классификации гражданских и военных самолётов.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/LjeDed/aircraft-classification/blob/main/notebooks/planes_classification.ipynb)

## Описание

Цель работы — сравнить возможности двух Vision-Language Models в задаче классификации изображений самолётов на два класса: `military` и `civil`.

В эксперименте использовались 30 изображений, включая простые и нетривиальные случаи.

## Используемые модели

- Qwen2.5-VL-3B-Instruct
- SmolVLM2-2.2B-Instruct

## Результаты

| Метрика | Qwen2.5-VL-3B | SmolVLM2-2.2B |
|---|---:|---:|
| Accuracy | **0.967** | 0.900 |
| Precision | 0.938 | **1.000** |
| Recall | **1.000** | 0.800 |
| F1-score | **0.968** | 0.889 |

Qwen2.5-VL показала более высокую общую точность и лучший результат на сложных изображениях.

## Структура проекта

```text
aircraft-classification/
├── assets/
├── notebooks/
│   └── planes_classification.ipynb
├── results/
├── .gitignore
└── requirements.txt
```

## Запуск

1. Откройте ноутбук через кнопку Open in Colab.
2. Подготовьте архив с исходными изображениями.
3. При необходимости включите GPU.
4. Выполните ячейки ноутбука.

## Технологии

Python, PyTorch, Hugging Face Transformers, Google Colab, Pandas, NumPy, Matplotlib, Scikit-learn.
