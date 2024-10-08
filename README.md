# Приложение для визуализации движения точки на ободе колеса

## Описание

Данное приложение реализует визуализацию движения точки на ободе колеса или диска. Пользователь может задавать параметры радиуса колеса и скорости центра масс, чтобы наблюдать траекторию движения точки. Приложение поддерживает две модели: статическую и динамическую.

- **Динамическая модель**: Отрисовка движения точки на ободе колеса с течением времени, создавая анимацию кривой.
- **Статическая модель**: График зависимости координаты y от x для траектории точки, без анимации.

## Входные параметры

- **Радиус колеса** (в метрах)
- **Скорость центра масс** (в метрах в секунду)

## Установка

### Требования

- Python 3.x
- PyQt5
- Matplotlib
- NumPy

### Инструкция по установке

1. Склонируйте репозиторий:

    ```bash
    git clone https://github.com/ArtemPustunniy/Fiz_task_3
    ```

2. Установите необходимые зависимости:

    ```bash
    pip install pyqt5 matplotlib numpy
    ```

3. Запустите приложение:

    ```bash
    python main.py
    ```

## Как использовать

1. Запустите приложение.
2. Введите радиус колеса и скорость центра масс в соответствующие поля.
3. Выберите модель: динамическую или статическую.
4. Нажмите кнопку "Перейти к отрисовке графика" для визуализации:
   - **Динамическая модель**: покажет анимацию движения точки на ободе колеса.
   - **Статическая модель**: отобразит график траектории точки.

## Структура проекта

- **MainWindow**: Основной класс приложения, который отвечает за интерфейс PyQt5 и визуализацию с помощью Matplotlib.
  - `static_model()`: Статическая отрисовка траектории движения точки.
  - `dynamic_model()`: Анимация движения точки по ободу колеса.

