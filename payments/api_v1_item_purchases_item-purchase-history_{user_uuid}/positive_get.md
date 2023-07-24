### Payments
#### Item purchases item purchase history {user_uuid} (positive)

Тестовые данные: https://payments.alpha.g-spot.website/v1/item_purchases/item-purchase-history/{user_uuid}/

Предусловие: user_uuid должен быть создан

1. Создать новый запрос в Postman
2. Выбрать метод GET для Request
3. Ввести URL: https://payments.alpha.g-spot.website/v1/item_purchases/item-purchase-history/86adbc1c-2924-4145-884d-b1f2c653bdd0/
4. Отправить Request

Ожидаемый результат: Server response: status code 200 - OK

Body response (в случае, если никаких выплат не было):

{
    "count": 0,
    "next": null,
    "previous": null,
    "results": []
}


Постусловие: удалить тестовые данные

Автор: Евгений

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-07-21 | 12:00 | Passed | Евгений | - | 