# Лабораторая работа №1 

## Задание: 
Написать программу на языке C/C++ для перемножения двух матриц
Исходные данные: файл(ы) содержащие значения исходных матриц
Выходные данные: файл со значениями результирующей матрицы, время выполнения, объем задачи

## Ключевые файлы: 
1. Cгенерированны матрицы в папке `matrices` разных размеров
2. Результат перемножение матриц в папке `results`
3. Файл статистики: `Info`
4. Файл проверки совпадения матриц: `results_py.txt`
5. Время затраченное на каждую операцию записывается в файл `consumed_time`

### Структура Multiply.cpp
1. Функция writeMatrix - записывает матрицу в файл
2. Функция readMatrix - читает матрицу из файла
3. Функция randomMatrix - генерирует матрицу заданного размера
4. Функция multiplyMatrix - перемножает матрицы и возвращает результат
5. В функции main происходит инициализация списка размеров матриц, создание двух случайных матриц, их умножение, запись результата в файл и замер времени выполнения операции для каждого размера матрицы

### Структура verify.py
1. Функция - load_matrix считывает матрицу из файла
2. Выполняется последовательная загрузка матриц из папки и их перемножение
3. Проводится проверка полученных результатов на соответствие

### Содержание файла  `consumed time.txt`
```
Mатрицы 100 - совпадают
Mатрицы 200 - совпадают
Mатрицы 500 - совпадают
Mатрицы 1000 - совпадают
Mатрицы 1500 - совпадают
Mатрицы 2000 - совпадают
Mатрицы 3000 - совпадают
```

## Вывод
При последовательном выполнении подсчета произведения двух матриц, время увеличивается с экспоненциальной зависимостью от количества элементов

