### Payments
#### Payment_accounts_owner_positive_input_valid_value_payout_day_of_month_PATCH

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/


1. Создать новый запрос в Postman, выбрать метод PATCH

2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/

3. Выбрать вкладку body=>тип raw=> формат JSON

4. Вставить данные в окно ввода
{
  "commission": "70",
  "frozen_time": "08:22:05",
  "gift_time": "03:36:11",
  "payout_day_of_month": 18
}

5. Ввести валидное значение в поле "payout_day_of_month"

6. Нажать кнопку “Send”

Ожидаемый результат: Server response status code 200 ok

Body response:
{
    "id": 1,
    "revenue_currency": "RUB",
    "revenue": "0.00",
    "income_currency": "RUB",
    "income": "0.00",
    "commission": "70.00",
    "frozen_time": "08:22:05",
    "gift_time": "03:36:11",
    "payout_day_of_month": 29
}

Постусловие: удалить тестовые данные

Автор: Василий

Тест выполнен
|     Дата    | Время | Результат |   Имя  | Баг №Trello|
|     ---     |  ---  |    ---    |   ---  |    ---     |
|  2023-07-18 | 17:12 |   Passed  | Василий|     -      | 