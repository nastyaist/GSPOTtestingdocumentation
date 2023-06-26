### Games reference
#### Get subgenre list


1. Запустить Postman
2. Создать запрос
- метод - GET
- URL - games.alpha.g-spot.website/api/v1/reference/subgenre/
3. Вкладка Authorization
Авторизоваться, используя [данные](https://github.com/victoretc/GSPOTtestingdocumentation/blob/main/Authorization_data.md).
5. Отправить запрос

Ожидаемый результат:
1. Status ответа: 200 OK.

2. В теле ответа вернулся список поджанров. Пример:

```
{
count*	integer
next	string($uri)
x-nullable: true
previous	string($uri)
x-nullable: true
results*	[SubGenre{
id	integer
title: ID
readOnly: true
name*	string
title: Subgenre
maxLength: 50
minLength: 1
 
}]
 
}

Автор: Ксения


| Дата | Время | Результат | Имя | Баг №  |
| ---  | ---   | ---       | --- | ---    |
|      |       |           |     |        | 
