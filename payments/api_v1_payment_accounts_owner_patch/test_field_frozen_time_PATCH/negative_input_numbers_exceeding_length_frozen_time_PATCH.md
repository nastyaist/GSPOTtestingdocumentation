### Payments
#### Payment_accounts_owner_positive_input_numbers_exceeding_length_frozen_time_PATCH

Тестовые данные: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/


1. Создать новый запрос в Postman, выбрать метод PATCH

2. Ввести URL: https://payments.alpha.g-spot.website/api/v1/payment_accounts/owner/

3. Выбрать вкладку body=>тип raw=> формат JSON

4. Вставить данные в окно ввода
{
  "commission": "33",
  "frozen_time": "11:11:11",
  "gift_time": "9:36:11",
  "payout_day_of_month": 21
}

5. Ввести кол-во цифр превышающие длинну в поле "frozen_time" (пример "12 11:05:33.666666344555555555555555555555555553")

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
|  2023-07-23 | 12:52 |   Passed  | Василий|     -      | 