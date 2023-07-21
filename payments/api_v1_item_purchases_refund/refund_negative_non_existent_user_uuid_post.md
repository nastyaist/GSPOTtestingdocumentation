### Payments
#### Item purchases refund (positive)

Тестовые данные: https://payments.alpha.g-spot.website/v1/item_purchases/refund/

Предусловие: user_uuid должен быть создан

1. Создать новый запрос в Postman
2. Выбрать метод POST для Request
3. Ввести URL: https://payments.alpha.g-spot.website/v1/item_purchases/refund/
4. Ввести в Body -> raw -> JSON:

{
  "user_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "item_uuid": "3fa85f64-5717-4562-b3fc-2c963f66afa6"
}

5. Отправить Request

Ожидаемый результат: Server response: status code 404 - not found

Body response:

{
    "detail": "No such product in this user."
}


Постусловие: удалить тестовые данные

Автор: Евгений

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-07-21 | 13:30 | Passed | Евгений | - | 