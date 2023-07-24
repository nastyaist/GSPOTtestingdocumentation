### Payments
#### Payment_accounts_owner_negative_input_spaces_frozen_time_PUT

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/


1. Создать новый запрос в Postman, выбрать метод PUT

2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/

3. Выбрать вкладку body=>тип raw=> формат JSON

4. Вставить данные в окно ввода
{
  "commission": "33",
  "frozen_time": "11:11:11",
  "gift_time": "9:36:11",
  "payout_day_of_month": 23
}

5. Ввести пробелы в поле "frozen_time" (пример "   ")

6. Нажать кнопку “Send”

Ожидаемый результат: Server response status code 400 Bad Request


Body response:
{
    "frozen_time": [
        "Duration has wrong format. Use one of these formats instead: [DD] [HH:[MM:]]ss[.uuuuuu]."
    
}

Постусловие: удалить тестовые данные

Автор: Василий

Тест выполнен
|     Дата    | Время | Результат |   Имя  | Баг №Trello|
|     ---     |  ---  |    ---    |   ---  |    ---     |
|  2023-07-23 | 12:25 |   Passed  | Василий|     -      | 