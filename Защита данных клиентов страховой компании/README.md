# Защита данных клиентов страховой компании

## Задача
Разработать метод преобразования данных, чтобы по ним было сложно восстановить персональную информацию. При этом после преобразования данных качество моделей машинного обучения не должно ухудшиться.
## Вывод
По условиям задачи необходимо было разработать алгоритм преобразования данных, чтобы по ним было сложно востановить персональную информацию о клиентах.

По формулам обучения модели "Линейная регрессия" было установлено, что при умножении признаков (данных о клиентах) на обратимую квадратную матрицу, значения предсказаний модели не изменяться. Также было установлено, что по произведению матрциы признаков и обратимой квадратнйо матрицы сложно восстановить исходную информацию.

На основе этих выводов был разработан **алгоритм преобразования данных**:
- Преобразовать признаки в матрицу F
- Создать квадратную обратимую матрицу P из случайных чисел размеро n x n, где n - ширина матрицы признаков F
- Умножить матрицу признаков F на обратимую матрицу P
- Преобразовать целевой признаки в вектор t

## Используемые инструменты
Pandas, NumPy, Scikit-learn
## Статус проекта
**Завершен**

