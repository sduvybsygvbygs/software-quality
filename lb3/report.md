# Лабораторна робота №3

## Модульне тестування програмного коду за допомогою Vitest

**Виконав: Пилипенко Артемій Валерійович**  
**Група: 6.1213-2пі**  
**Дата: 06.10.2026**

## Test Object

`src/shop-utils.js`

## Функції

- `calculateDiscount()`
- `validateQuantity()`
- `getShippingCost()`

## Test Design

### calculateDiscount

Для перевірки коректного розрахунку ціни зі знижкою був використаний наступний набір даних:

| price | discount |
|-------|---------:|
| 100   |       10 |
| 100   |        0 |
| 100   |      100 |

Для перевірки коректної реакції на недопустимі значення price та discount було використано наступний набір даних:

| price | discount |
|-------|---------:|
| -10   |       10 |
| 10    |      -10 |

### validateQuantity

Equivalence partitions:

| Значення     | Partition  | Expected |
|--------------|----------:|----------|
| < 1          |     Invalid      |     false     |
| 1-10, integer |         Valid   |       true   |
| > 10         |      Invalid     |      false    |
| не ціле число |       Invalid    |       false   |

Boundary values:

| Quantity | Expected |
|----------|------:|
| 0        |   false    |
| 1        |     true  |
| 2        |     true  |
| 9        |    true   |
| 10       |     true  |
| 11       |    false   |
| 1.5      |   false    |


### getShippingCost

Перевірені гілки:

1. if (!Number.isFinite(total) || total < 0)

2. if (total >= 1000)

## Результати тестування

| Група тестів | Кількість | Result |
|---|----------:|--------|
| calculateDiscount |         5 | 5/5    |
| validateQuantity |         7 | 7/7    |
| getShippingCost |         3 | 3/3    |

## Coverage

| Metric | Result |
|---|-------:|
| Statements |    100 |
| Branches |    100 |
| Functions |    100 |
| Lines |    100 |

## Висновок

У ході виконання лабораторної роботи було опрацьовано принципи модульного тестування програмного коду за допомогою Vitest. Було створено та виконано unit-тести для функцій calculateDiscount(), validateQuantity() та getShippingCost(). За результатами запуску тестів було перевірено правильність роботи функцій та проаналізовано покриття коду тестами.