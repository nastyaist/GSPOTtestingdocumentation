Payments

PAYOUT DATA

Тестовые данные: 
https://payments.alpha.g-spot.website/api/v1/payment_accounts/payout_data/3fa85f64-5717-4562-b3fc-2c963f66afa6/

1.Создать новый запрос в Postman

2.Выбрать метод PUT для Request

3.Ввести URL:
https://payments.alpha.g-spot.website/api/v1/payment_accounts/payout_data/3fa85f64-5717-4562-b3fc-2c963f66afa6/

4.Ввести в Body -> raw -> JSON:  

{
  "account_number": "string",
  "is_auto_payout": true,
  "payout_type": "bank_card"
}
Отправить Request

Ожидаемый результат: 200 ok

{
  "account_number": "string",
  "is_auto_payout": true,
  "payout_type": "bank_card"
}

Постусловие: удалить тестовые данные 

Автор: Юлия

Тест выполнен

22.07.2023
