## Домашнее задание к занятию 12.1. «Базы данных» - `Виноградова Татьяна`

---

### Задание 1.

### Структура таблиц базы данных:

#### 1. Сотрудники
```
{
Сотрудник_id, первичный ключ, serial,
Фамилия, varchar(50),
Имя,  varchar(50),
Отчество, varchar(50),
Идентификатор должности, внешний ключ, integer,
Идентификатор структурного подразделения, внешний ключ, integer,
Идентификатор адреса филиала, внешний ключ, integer,
Оклад, money,
Дата найма, date
}
```

#### 2. Должности 
```
{
Должность_id,  первичный ключ, serial,
Наименование должности,  varchar(50))
}
```
#### 3. Типы подразделений
```
{
Тип_подразделения_id,  первичный ключ, serial,
Наименование типа подразделения,  varchar(50))
}
```
#### 4. Подразделения 
```
{
Подразделение_id, первичный ключ, serial,
Идентификатор типа подразделения, внешний ключ, integer,
Наименование подразделения,  varchar(50))
}
```
#### 5. Регионы
```
{
Регион_id, первичный ключ, serial,
Название региона, varchar(50)
}
```
#### 6. Города
```
{
Город_id, первичный ключ, serial,
Идентификатор региона, внешний ключ, integer,
Название города, varchar(50)
}
```
#### 7. Улицы
```
{
Улица_id, первичный ключ, serial,
Идентификатор города, внешний ключ, integer,
Название улицы, varchar(100)
}
```
#### 8. Адрес филиала
```
{
Адрес_филиала_id, первичный ключ, serial,
Идентификатор региона, внешний ключ, integer,
Идентификатор города, внешний ключ, integer,
Идентификатор улицы, внешний ключ, integer,
Номер дома, varchar(20)
}
```
#### 9. Проекты
```
{
Проект_id, первичный ключ, serial,
Название проекта, varchar(100)
}
```
#### 10. Назначенные проекты
```
{
Назначенный_проект_id, первичный ключ, serial,
Идентификатор проекта, внешний ключ, integer,
Идентификатор сотрудника, внешний ключ, integer,
}
```


