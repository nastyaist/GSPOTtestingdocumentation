### Payments
#### Payment_accounts_owner_positive_input_valid_value_in_all_params_PUT

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/


1. Создать новый запрос в Postman, выбрать метод PUT

2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/

3. Выбрать вкладку body=>тип raw=> формат JSON

4. Вставить данные в окно ввода
{
  "commission": "344",
  "frozen_time": "00:00:00",
  "gift_time": "00:00:00",
  "payout_day_of_month": 13
}

5. Ввести валидные значения во все параметры

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
    "frozen_time": "10:01:20",
    "gift_time": "09:36:11",
    "payout_day_of_month": 23
}

Постусловие: удалить тестовые данные

Автор: Василий

Тест выполнен
|     Дата    | Время | Результат |   Имя  | Баг №Trello|
|     ---     |  ---  |    ---    |   ---  |    ---     |
|  2023-07-18 | 16:52 |   Passed  | Василий|     -      | 