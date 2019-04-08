# MySQL_IC_HomeWorks
MySQL_IC_HomeWorks Базы данных. Интерактивный курс 2018/09/18

Урок 2 - Язык запросов SQL
1. Пусть в таблице catalogs базы данных shop в строке name могут находиться пустые строки и поля, принимающие значение NULL. Напишите запрос, который заменяет все такие поля на строку ‘empty’. Помните, что на уроке мы установили уникальность на поле name. Возможно ли оставить это условие? Почему?
2. Спроектируйте базу данных, которая позволяла бы организовать хранение медиафайлов, загружаемых пользователем (фото, аудио, видео). Сами файлы будут храниться в файловой системе, а база данных будет содержать только пути к файлам, названия, описания, ключевых слов и принадлежности пользователю.
3. (по желанию) В учебной базе данных shop присутствует таблица catalogs. Пусть в базе данных sample имеется таблица cat, в которой могут присутствовать строки с такими же первичными ключами. Напишите запрос, который копирует данные из таблицы catalogs в таблицу cat, при этом для записей с конфликтующими первичными ключами в таблице cat должна производиться замена значениями из таблицы catalogs.


Урок 3 - Операторы, фильтрация, сортировка и ограничение
1. Пусть в таблице users поля created_at и updated_at оказались незаполненными. Заполните их текущими датой и временем.
2.Таблица users была неудачно спроектирована. Записи created_at и updated_at были заданы типом VARCHAR и в них долгое время помещались значения в формате "20.10.2017 8:10". Необходимо преобразовать поля к типу DATETIME, сохранив введеные ранее значения.
3. В таблице складских запасов storehouses_products в поле value могут встречаться самые разные цифры: 0, если товар закончился и выше нуля, если на складе имеются запасы. Необходимо отсортировать записи таким образом, чтобы они выводились в порядке увеличения значения value. Нулевые запасы должны выводиться в конце, после всех записей.
4. (по желанию) Из таблицы users необходимо извлечь пользователей, родившихся в августе и мае. Месяцы заданы в виде списка английских названий ('may', 'august')
5. (по желанию) Из таблицы catalogs извлекаются записи при помощи запроса. SELECT * FROM catalogs WHERE id IN (5, 1, 2); Отсортируйте записи в порядке, заданном в списке IN.


Урок 4 - Агрегация данных
1. Подсчитайте средний возраст пользователей в таблице users.
2. Подсчитайте количество дней рождения, которые приходятся на каждый из дней недели. Следует учесть, что необходимы дни недели текущего года, а не года рождения.
3. (по желанию) Подсчитайте произведение чисел в столбце таблицы.

Урок 5 - Сложные запросы
1. Составьте список пользователей users, которые осуществили хотя бы один заказ (orders) в интернет-магазине.
2. Выведите список товаров products и разделов catalogs, который соответствует товару.
3. (по желанию) Есть таблица рейсов flights (id, from, to) и таблица городов cities (label, name). Поля from, to и label содержат английские названия городов, поле name — русское. Выведите список рейсов (flights) с русскими названиями городов.
