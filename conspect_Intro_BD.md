# CУБД — СИСТЕМА УПРАВЛЕНИЯ БАЗАМИ ДАННЫХ

CУБД – _ИНСТРУМЕНТ_

Базы данных:

- Картотека
- Библиотека
- Результаты переписи
- Книга учета

*Базы данных нужны для:*
- хранения, 
- обработки,
- быстрого извлечения необходимой информации.

## Виды баз данных:

## 1. Иерархическая модель хранения данных

При создании иерархической базы данных мы изначально фиксируем сценарий использования этой базы
Иерархическая модель удобна, если она создаётся под конкретную задачу. 

***Пример – предметный указатель***

## 2. Реляционные базы данных 
– это базы данных, в которых
данные распределены по отдельным, связанным
между собой, таблицам.

- Первичный ключ — ID, уникальная информация, которая позволяет идентифицировать каждую конкретную запись таблицы.
- Внешний ключ — ID из дополнительной таблицы (уже не уникальный). Позволяет найти информацию из основной таблицы.

Реляционные базы данных (от англ. Relation – связь) — базы данных, в которых данные распределены по отдельным, но связанным между собой таблицам.

***Пример - телефонный справочник.***

# Псевдокод SQL 
SQL – это особый язык программирования, который позволяет формулировать то,
что нужно сделать с данными в таблицах.

1. SELECT * FROM Общий список

- Select (англ. «выбери») — команда, в которой мы указываем, что выбираем.
- (*) означает, что мы хотим видеть все столбцы, которые есть в таблице, указанной дальше. Вместо звёздочки можно указать конкретные столбцы, если по условию задачи нужно выбрать их.
- From (англ. «из») — откуда мы извлекаем данные.

Соответственно, команда звучит так: «Выбери все столбцы из». А дальше указываем название таблицы, из которой хотим получить эти данные, — «Общий список».

## Извлечение данных из таблиц может осуществляться следующими способами:

- INNER JOIN - Это самый распространенный тип объединения. С его помощью происходит объединение записей из двух таблиц по связующему полю, если оно содержит одинаковые значения в обеих таблицах.
- LEFT JOIN - Операция LEFT JOIN создает левое внешнее соединение. С помощью левого внешнего соединения выбираются все записи первой (левой) таблицы, даже если они не соответствуют записям во второй (правой) таблице.
- RIGHT JOIN - Операция RIGHT JOIN создает правое внешнее соединение. С помощью правого внешнего соединения выбираются все записи первой (правой) таблицы, даже если они не соответствуют записям во второй (левой) таблице.
- FULL JOIN - Он объединяет результаты как левого, так и правого внешних соединений. Объединенная таблица будет содержать все записи из обеих таблиц и заполнять NULL для отсутствия совпадений с обеих сторон.

## Структура базы данных.

Структура базы данных может определяться видами связей:

- Один к одному (За номером закреплен лишь один клиент)
- Один ко многим (У одного клиента может быть несколько номеров)
- Многие ко многим (Одна книга могла быть написана несколькими авторами.
Автор мог написать несколько книг)
