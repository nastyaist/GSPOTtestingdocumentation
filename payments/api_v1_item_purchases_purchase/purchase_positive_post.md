### Payments
#### Item purchases purchase (positive)

Тестовые данные: https://payments.alpha.g-spot.website/v1/item_purchases/purchase/

Предусловие: user_uuid должен быть создан

1. Создать новый запрос в Postman
2. Выбрать метод POST для Request
3. Ввести URL: https://payments.alpha.g-spot.website/v1/item_purchases/purchase/
4. Ввести в Body -> raw -> JSON:

{
  "payment_type": "bank_card",
  "payment_service": "yookassa",
  "user_uuid_from": "52b71907-60c9-4602-a7aa-b53ff78aaba6",
  "user_uuid_to": "52b71907-60c9-4602-a7aa-b53ff78aaba6",
  "items_payment_data": [
    {
      "item_uuid": "52b71907-60c9-4602-a7aa-b53ff78aaba6",
      "developer_uuid": "52b71907-60c9-4602-a7aa-b53ff78aaba6",
      "price": {
        "amount": "100",
        "currency": "RUB"
      }
    }
  ],
  "return_url": "https://example.com/",
  "price_with_commission": {
    "amount": "103.63",
    "currency": "RUB"
  }
}

5. Отправить Request

Ожидаемый результат: Server response: status code 201 - ok

Body response:

{
  "payment_type": "bank_card",
  "payment_service": "yookassa",
  "user_uuid_from": "52b71907-60c9-4602-a7aa-b53ff78aaba6",
  "user_uuid_to": "52b71907-60c9-4602-a7aa-b53ff78aaba6",
  "items_payment_data": [
    {
      "item_uuid": "52b71907-60c9-4602-a7aa-b53ff78aaba6",
      "developer_uuid": "52b71907-60c9-4602-a7aa-b53ff78aaba6",
      "price": {
        "amount": "100",
        "currency": "RUB"
      }
    }
  ],
  "return_url": "https://example.com/",
  "price_with_commission": {
    "amount": "103.63",
    "currency": "RUB"
  }
}


Постусловие: удалить тестовые данные

Автор: Евгений

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-07-21 | 13:00 | Failed | Евгений | Баг не заводился, тк для ручки нужно подключить Юкассу | 