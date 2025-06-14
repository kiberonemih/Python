# Урок 8

## Функции

Функции — это блоки кода, которые:
1. Выполняют определенные операции
2. Могут принимать входные параметры (аргументы)
3. Могут возвращать результат вычислений

Функции позволяют избежать дублирования кода

> "Функция создает маленькую программу для её повторного использования в основной программе"

## Создание собственных функций

### Синтаксис
```python
def имя_функции(параметры):
    # Тело функции
    return результат 
```

## Примеры

### Простая функция без параметров
```python
def welcome():
    print("Hello!")

welcome()  # Вызов функции
```

### Функции с параметрами
```python
def welcome(name):
    print(f"Hello, {name}!")
    
welcome("Boris")  # Hello, Boris!
```

### Функции с возвращаемым значением
```python
def add(a, b):
    return a + b
    
result = add(3, 5)  # result = 8
```



## Рекомендации
1. **Имена функций должны быть описательными**
2. **Одна функция - одна задача**
3. **Функции должны быть короткими** (желательно не более 10-15 строк)
