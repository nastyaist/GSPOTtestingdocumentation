### Payments
#### Payment_accounts_owner_positive_input_value_with_dot_and_two_decimal_places_comission_PATCH

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/


1. Создать новый запрос в Postman, выбрать метод PATCH

2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/

3. Выбрать вкладку body=>тип raw=> формат JSON

4. Вставить данные в окно ввода
{
  "commission": "344",
  "frozen_time": "00:00:00",
  "gift_time": "00:00:00",
  "payout_day_of_month": 16
}

5. Ввести значение с точкой и 2 знака полсе в поле "commission"-(пример "1.66")

6. Нажать кнопку “Send”

Ожидаемый результат: Server response status code 200 ok

Body response:
{
    "id": 1,
    "revenue_currency": "RUB",
    "revenue": "0.00",
    "income_currency": "RUB",
    "income": "0.00",
    "commission": "1.66",
    "frozen_time": "00:00:00",
    "gift_time": "00:00:00",
    "payout_day_of_month": 16
}

Постусловие: удалить тестовые данные

Автор: Василий

Тест выполнен
|     Дата    | Время | Результат |   Имя  | Баг №Trello|
|     ---     |  ---  |    ---    |   ---  |    ---     |
|  2023-07-23 | 16:10 |   Passed  | Василий|     -      | 