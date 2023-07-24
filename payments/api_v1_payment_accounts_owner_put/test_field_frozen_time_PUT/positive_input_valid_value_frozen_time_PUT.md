### Payments
#### Payment_accounts_owner_positive_input_valid_value_frozen_time_PUT

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/


1. Создать новый запрос в Postman, выбрать метод PUT

2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/

3. Выбрать вкладку body=>тип raw=> формат JSON

4. Вставить данные в окно ввода
{
  "commission": "33",
  "frozen_time": "11:11:11",
  "gift_time": "9:36:11",
  "payout_day_of_month": 21
}

5. Ввести валидное значение в поле "frozen_time"

6. Нажать кнопку “Send”

Ожидаемый результат: Server response status code 200 ok

Body response:
{
    "id": 1,
    "revenue_currency": "RUB",
    "revenue": "0.00",
    "income_currency": "RUB",
    "income": "0.00",
    "commission": "33.00",
    "frozen_time": "11:11:11",
    "gift_time": "09:36:11",
    "payout_day_of_month": 21
}

Постусловие: удалить тестовые данные

Автор: Василий

Тест выполнен
|     Дата    | Время | Результат |   Имя  | Баг №Trello|
|     ---     |  ---  |    ---    |   ---  |    ---     |
|  2023-07-23 | 12:15 |   Passed  | Василий|     -      | 