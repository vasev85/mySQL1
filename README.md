# Домашнее задание к занятию 12.2 "Работа с данными (DDL/DML)"

Домашнее задание выполните в Google Docs и отправьте в личном кабинете на проверку ссылку на ваш документ.

Название файла должно содержать номер лекции и фамилию студента. Пример названия: "12.2 Работа с данными (DDL/DML) - Александр Александров"

Перед тем как выслать ссылку, убедитесь, что ее содержимое не является приватным (открыто на просмотр всем, у кого есть ссылка). Если необходимо прикрепить дополнительные ссылки, просто добавьте их в свой Google Docs.

Любые вопросы по решению задач задавайте в чате учебной группы.


---

Задание можно выполнить как в любом IDE, так и в командной строке.

### Задание 1.
1.1 Поднимите чистый инстанс MySQL версии 8.0+. Можно использовать локальный сервер или контейнер Docker.

1.2 Создайте учетную запись sys_temp. 

1.3 Выполните запрос на получение списка пользователей в Базе Данных. (скриншот)

![alt text](https://github.com/vasev85/mySQL1/blob/main/screens/ex1.png?raw=true)


1.4 Дайте все права для пользователя sys_temp. 

1.5 Выполните запрос на получение списка прав для пользователя sys_temp. (скриншот)

![alt text](https://github.com/vasev85/mySQL1/blob/main/screens/ex1-2.png?raw=true)


1.6 Переподключитесь к базе данных от имени sys_temp.

Для смены типа аутентификации с sha2 используйте запрос: 
```sql
ALTER USER 'sys_test'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';
```
1.6 По ссылке https://downloads.mysql.com/docs/sakila-db.zip скачайте дамп базы данных.

1.7 Восстановите дамп в базу данных.

1.8 При работе в IDE сформируйте ER-диаграмму получившейся базы данных. При работе в командной строке используйте команду для получения всех таблиц базы данных. (скриншот)

![alt text](https://github.com/vasev85/mySQL1/blob/main/screens/ex1-3.png?raw=true)


*Результатом работы должны быть скриншоты обозначенных заданий, а так же "простыня" со всеми запросами.*


### Задание 2.
Составьте таблицу, используя любой текстовый редактор или Excel, в которой должно быть два столбца, в первом должны быть названия таблиц восстановленной базы, 
во втором названия первичных ключей этих таблиц. Пример: (скриншот / текст)
```
Название таблицы | Название первичного ключа
customer         | customer_id
```


## Дополнительные задания (со звездочкой*)
Эти задания дополнительные (не обязательные к выполнению) и никак не повлияют на получение вами зачета по этому домашнему заданию. Вы можете их выполнить, если хотите глубже и/или шире разобраться в материале.

### Задание 3.*
3.1 Уберите у пользователя sys_temp права на внесение, изменение и удаление данных из базы sakila.

3.2 Выполните запрос на получение списка прав для пользователя sys_temp. (скриншот)

![alt text](https://github.com/vasev85/mySQL1/blob/main/screens/ex3.png?raw=true)


*Результатом работы должны быть скриншоты обозначенных заданий, а так же "простыня" со всеми запросами.*
