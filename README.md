# Телеграм-бот "Гороскоп"

Этот проект представляет собой телеграм-бота, который предоставляет пользователям гороскопы на каждый день. Бот написан на Python с использованием библиотеки aiogram.

## Функционал

- **Выбор знака зодиака**: При регистрации бот предлагает пользователю выбрать свой знак зодиака с помощью кнопок, оформленных в виде эмоджи. Кнопки организованы в 3 ряда по 4 кнопки.
  
- **Гороскоп на сегодня**: После выбора знака зодиака бот отправляет гороскоп на текущий день, который включает текст, картинку и кнопку "Обновить". Текст гороскопа содержит дату, выделенную жирным шрифтом. При нажатии на кнопку "Обновить" сообщение обновляется, и прогноз изменяется на новый.

- **Автоматическое обновление**: Каждый день в 10 утра бот автоматически отправляет пользователю новый гороскоп, если его еще нет.

- **Команда /update**: Пользователь может вручную обновить гороскоп на сегодня с помощью команды `/update`. Это аналогично нажатию на кнопку "Обновить".

- **Команда /change_zodiac**: Позволяет пользователю изменить свой знак зодиака. При нажатии на команду появляется клавиатура, как при регистрации, и после выбора нового знака зодиака бот отправляет новый гороскоп.

- **Команда /clear_history**: Очищает историю сообщений, оставляя только сообщение с последним выбранным знаком зодиака.

- **Обработка неизвестных сообщений**: Если пользователь отправляет сообщение, которое бот не понимает, он отвечает: "Извините, я не понял".

## Установка

1. Убедитесь, что у вас установлен Python 3.7 или выше.
2. Установите необходимые библиотеки:
3. Получите токен для вашего бота у BotFather и замените YOUR_API_TOKEN_HERE в коде на ваш токен.

## Запуск
Для запуска бота выполните следующую команду:
```bash
python3 your_bot_file.py
```
Где your_bot_file.py — это имя файла, в котором находится ваш код бота.

## Использование
После запуска бота вы можете начать с командой /start, выбрать свой знак зодиака, и бот начнет отправлять вам гороскопы.
