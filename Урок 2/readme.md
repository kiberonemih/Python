# Урок 2

## Строки (`str`)
Определение: последовательность символов, заключённая в кавычки:

 - Двойные: `"Текст"` (Shift + 2 на русской раскладке)

 - Одинарные: `'Текст'` (клавиша `Э` на английской раскладке)

 - Тройные: 
 ```
 '''
 Многострочный 
 текст
 '''
 ```

Пример:
  ```python
  print("Hello, World!")  # Вывод строки
  ```

## Экранирование символов

`\\` — обратный слеш.

`\'` — одинарная кавычка.

`\"` — двойная кавычка.

`\n` — перенос строки.

`\t` — табуляция.

`\a` — звук системного динамика.

Пример: 

```python
print("Путь к файлу: \"C:\\folder\\file.py\"")  # Экранирование кавычек и слешей
# Вывод: "Путь к файлу: "C:\folder\file.py""
```

## Операции со строками

### Сложение:
  ```python
  str1 = "Hello"
  str2 = "World"
  print(str1 + " " + str2)  # Вывод: "Hello World"
  ```
  Важно: нельзя складывать строку с числом без преобразования (`str(число)`).

### Умножение строк:
  ```python
  print("Повтор " * 3)  # Вывод: "Повтор Повтор Повтор "
  ```
  Умножение на `0` даёт пустую строку, на отрицательные числа — ошибку.


## Форматирование строк
f-строки (рекомендуемый способ):
  ```python
  name = "Анна"
  age = 25
  print(f"Меня зовут {name}, мне {age} лет.")  # Вывод: "Меня зовут Анна, мне 25 лет."
  ```
  Позволяют вставлять переменные прямо в текст через `{ }`.

Преобразование типов:
  ```python
  number = 10
  text = str(number)  # Преобразование числа в строку
  ```

## Ввод данных 

`input()` — функция для получения данных от пользователя прямо во время выполнения программы. Программа ждёт, пока пользователь введёт текст и нажмёт Enter

В скобки можно добавить подсказку, которая выведется перед тем как начать ждать ввод пользователя

Пример:
```python
name = input("Введите ваше имя: ")
age = input("Введите ваш возраст: ")
print(f"Меня зовут {name}, мне {age} лет.")
```

`input()` возвращает введённые данные как строку (`str`).

Для чисел используйте int() или float():

```python
num1 = int(input("Введите число 1: "))
num2 = int(input("Введите число 2: "))
print(f"Сумма: {num1 + num2}")
```