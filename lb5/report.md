# Лабораторна робота №5
## Інтеграційне тестування компонентів та зовнішніх систем
**Виконав: Пилипенко Артемій Валерійович**
**Група: 6.1213-2пі**
**Дата: 03.11.2026**
## 1. Component Integration Testing
### Test Object
`CartService <-> shop-utils`
### Scenario 1 — Discount
Test Data:
- item 1: price = 100;
- item 2: price = 200;
- discount = 10%.
  Expected Result:
  `270`
  Actual Result:
  `270`
  Result:
  `Pass`
### Scenario 2 — Invalid Discount
Test Data:
- item: price = 100;
- discount = 110%.
  Expected Result:
  `Discount must be between 0 and 100`
  Actual Result:
  `Discount must be between 0 and 100`
  Result:
  `Pass`
## 2. System Integration Testing
### Test Object
`ExternalEchoGateway ↔ Postman Echo`
### Test Data
- orderId = `ORD-001`;
- total = `270`.
### Expected Result
```json
{
"orderId": "ORD-001",
"total": 270
}
```
## Висновк
В ході виконання лабораторної роботи створено інтеграційні тести для взяємодії програмних компонентів та інтеграції з зовнішньою системою. Було отримано теоретичні та практичні навички для коректної класифікації та реалізації тестів.