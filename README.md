Всем привет! Эта инструкция и требования к сайту (localhostENG).
----------------------------------------------------------------------------------------------------------
Сервер баз данных
Мин версия сервера: 5.6.41 - MySQL Community Server (GPL)
Файл для соединения с БД сайта db.php сейчас стоит сервер:'localhost', пользователь:'mysql', пароль:'mysql', имя база данных:'medikusman'
Используемая ORM библиотека RedBeanPHP
Кодировка по умолчанию сервера: UTF-8 Unicode (utf8)

Веб-сервер
Apache
Мин версия PHP: 5.5.38

1. Распаковать архив с файлами в корне сайта
2. Указать данные связи с БД в файле db.php
3. Зарегистрироваться на сайте, войти, перейти на главную, после чего будет доступна админ панель
4. Выполнить SQL-запрос в таблице users
----------------------------------------------------------------------------------------------------------
INSERT INTO `users` (`id`, `name`, `surname`, `login`, `email`,`gender`, `dateborn`, `password`) VALUES  
 (4, 'Tom','Bruce','Driver','speed@mail.ru','Male', '2019-09-30', '123'),  
 (5, 'Clara','Gilliam','Programmer','Programmer@mail.ru','Female','1995-09-30','12345'),  
 (6, 'Barbra','Hurley', 'Female', 'Technician@mail.ru', 'Female','1998-03-19','23434'),  
 (7, 'Antonio', 'Forbes','Faller','Faller@mail.ru','Male','1992-08-28','3566'),  
 (8, 'Charles','Horst','Financial','Financial@mail.ru','Male','1991-07-13','345768'),  
 (9, 'Clayton','Beau','Extractive','Extractive@mail.ru','Male','1999-09-19','1236565'),   
 (10, 'Burns','Ramona','Electronic','Electronic@mail.ru','Male','1999-09-19','1236565');
-----------------------------------------------------------------------------------------------------------

Что не доработано:
1. Связка редактирования в соответсвии с сортировкой (на данный момент состоят раздельно)
2. Постраничное разделение
3. При редактировании записи пароль не будет актуален
4. При создание записи пароль не будет актуален
5. Пробелы в формах
