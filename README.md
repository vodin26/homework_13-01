#Домашнее задание к занятию «Кеширование Redis/memcached  "Воронин Владислав"»

### Задание 1

## Проблемы, решаемые кешированием:

1. **Задержки при запросах:** Кэширование позволяет быстро выдать данные из памяти компьютера вместо ожидания доступа к хранилищам на диске, что приводит к быстрому снижению задержек.
2. **Низкая производительность БД:** Бывает так, что базы данных имеют слишком много запросов, что приводит к низкой их производительности. Кэширование помогает справится с этими проблемами.
3. **Часто обновляемые данные:** Если в приложении часто появляются новые данные, то есть вероятность того, что старая информация может быть еще актуальной, поэтому кеширование позволяет хранить эту информацию в оперативной памяти.
4. **Большой объем данных:** При работе с огромным количеством данных возникает потребность в быстрой выдаче данных. Кэширование позволяет сохранять эти данные в более доступном и быстром месте.

**Примеры решаемых задач:**

1. **Постоянное обновление информации о пользователях:** В системе часто появляются новые пользователи, поэтому данные должны быть быстро актуализированы.
2. **Временные показатели метрик приложения:** Приложение имеет много метрики (например, количество активных пользователей в определенный момент времени), поэтому кэширование позволяет хранить эти данные в оперативной памяти.
3. **Справочники:** Кэширование можно использовать для сохраняния данных из справочников.
4. **Изучение базовых данных:** В некоторых случаях необходимо быстро найти и вывести данные из БД, поэтому кэширование может помочь.

**Возможные проблемы:**

1. **Переизбытие в памяти компьютера:** Если используемый кеширование имеет ограниченный объем, то возможен вариант, что данными в нем будет больше чем свободной памяти.
2. **Потеря актуальности данных:** Если данные в кэше долго не обновляются, то есть вероятность того, что они потерят свою актуальность.

**Возможные решения:**

1. **Кеширование на диске:** В случае, когда памяти компьютера недостаточно, кеширование можно хранить на диске.
2. **Использование более эффективного кэширования:** В современных приложениях часто используются эффективные технологии кеширования, которые позволяют экономить место в оперативной памяти.

В некоторых случаях кеширование может помочь решить вышеуказанные проблемы.

### Задание 2

![alt text](https://github.com/vodin26/homework_11-02/blob/main/img/pic_1.png)

### Задание 3

### Задание 4
