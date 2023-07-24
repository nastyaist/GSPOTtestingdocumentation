### Payments
#### Payment_accounts_owner_negative_input_numbers_exceeding_length_gift_time_PATCH

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/


1. Создать новый запрос в Postman, выбрать метод PATCH

2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/

3. Выбрать вкладку body=>тип raw=> формат JSON

4. Вставить данные в окно ввода
{
  "commission": "33",
  "frozen_time": "11:11:11",
  "gift_time": "19:36:11",
  "payout_day_of_month": 21
}

5. Ввести цифр превышающие кол-во длинны в поле "gift_time" (пример "30 19:36:11.3333336555555555555555555333)
6. Нажать кнопку “Send”

Ожидаемый результат: Server response status code 400 Bad Request


Body response:
{
    "gift_time": [
        "Duration has wrong format. Use one of these formats instead: [DD] [HH:[MM:]]ss[.uuuuuu]."
    
}

Постусловие: удалить тестовые данные

Автор: Василий

Тест выполнен
|     Дата    | Время | Результат |   Имя  | Баг №Trello|
|     ---     |  ---  |    ---    |   ---  |    ---     |
|  2023-07-24 | 14:46 |   Passed  | Василий|     -      | 