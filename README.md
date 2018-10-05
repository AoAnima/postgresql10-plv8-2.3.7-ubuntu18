## postgresql10-plv8-2.3.7-ubuntu18
#PLV8 для Postgresql 10, ubuntu 18.
Должен быть установлен libc++-dev 
```
sudo apt-get install libc++-dev
```
Содержимое каталога переносим в папку usr,
если из командной строки то переключаемся на пользователя postgres 

```
sudo su - postgres
```
входим в psql
```
psql
```
И создаём расширение
```
CREATE EXTENSION plv8;
```
Проверяем
```
SELECT plv8_version();
  plv8_version
-----------------
2.3.7
(1 row)
```
пользуемся
