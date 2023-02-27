Ревью литературы: https://docs.google.com/document/d/1LNh47_zyJ_B68mztQ7oIK3QrsUzjGO1lNtmeSeLOkLc/edit?usp=sharing

NLP problem prompt engineering with chain-of-thoughts
========
В исследовании рассматривается проблема решения арифметических задач при помощи языковых моделей. Предлагается метод chain-of-thoughts, который заключается в подаче промта-подсказки для модели, заставляющей модель проводить промежуточные размышления во время решения задачи. Также предлагается модификация метода self-consistency, предполагающий агрегацию нескольких различных решений задачи для повышения вероятности вывода правильного ответа.

Сетап эксперимента
===========
- Модель: Bloom-176B (https://huggingface.co/bigscience/bloom)
- Датасет: GSM8K (https://huggingface.co/datasets/gsm8k)
- Платформа для работы: Kaggle (https://www.kaggle.com/)

Запуск эксперимента
===========
Требуется установка библиотеки `petals`, это можно сделать командой `!pip install -q petals`
Также потребуются `torch`, `transformers`, `tqdm`. Для этого поможет команда `!pip install torch transformers tqdm`

Весь код собран в юпитер ноутбуке `main.ipynb` в папке `code`.

Результаты
=======
К сожеланию, собрать качественные результаты в процессе работы не удалось в связи с высокой загруженностью серверов инференса модели, однако эксперименты будет возможно воспроизвести если развернуть модель на своих серверах.