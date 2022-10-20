# Анализ мобильного приложения "Ненужные вещи"

## Проведем предобработку данных:

  - Датасеты проверим на дубликаты;
  
  - Датасеты проверим на пропуски;
  
  - Приведем названия столбцов в порядок(если потребуется);
  
  - Приведем к нужному типу дата и время(если потребуется)
  
## Проведем исследовательский анализ данных:

  - Узнаем, пользователи какой группы склонны часто возвращаться в мобильное приложение(RETENTION RATE);
  
  - Узнаем, пользователи какой группы часто делают целевое событие(конверсия в целевое действие);
  
  - Узнаем, как распределяется время между распространенными событиями пользователей из разных групп;
  
 
## Выделим сегменты пользователей для управления вовлеченностью:
  
  - Выделим целевую и смежную аудиторию;
  
  - Посмотрим частоту действий пользователей каждой группы по неделям.
  
  
## Сформулируем и проверим гипотезы:
  
  - Некоторые пользователи установили приложение по ссылке из yandex, другие — из google. Проверим гипотезу: две эти группы демонстрируют разную конверсию в просмотры контактов.
  
  - Сформулируем нулевую гипотезу:

     - Разницы в количестве событий, от общего числа событий, между группами нет
     
  - Сформулируем альтернативную гипотезу:   
     
     - Разница в количестве событий, от общего числа событий, между группами есть
     
     
## Напишем выводы и рекомендации

# **Описание данных:**

Датасет содержит данные о событиях, совершенных в мобильном приложении "Ненужные вещи". В нем пользователи продают свои ненужные вещи, размещая их на доске объявлений.

В датасете содержатся данные пользователей, впервые совершивших действия в приложении после 7 октября 2019 года.

Датасет **mobile_dataset.csv** содержит колонки:

- `event.time` — время совершения

- `event.name` — название события

- `user.id` — идентификатор пользователя

Датасет **mobile_sources.csv** содержит колонки:

- `userId` — идентификатор пользователя

- `source` — источник, с которого пользователь установил приложение

Расшифровки событий:

- `advert_open` — открытие карточки объявления

- `photos_show` — просмотр фотографий в объявлении

- `tips_show` — пользователь увидел рекомендованные объявления

- `tips_click` — пользователь кликнул по рекомендованному объявлению

- `contacts_show` и `show_contacts` — пользователь нажал на кнопку "посмотреть номер телефона" на карточке объявления

- `contacts_call` — пользователь позвонил по номеру телефона на карточке объявления

- `map` — пользователь открыл карту размещенных объявлений

- `search_1` — `search_7` — разные события, связанные с поиском по сайту

- `favorites_add` — добавление объявления в избранное
