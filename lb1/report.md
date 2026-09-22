\# Лабораторна робота №1





\## Аналіз якості програмного продукту. Виявлення та документування аномалій





\*\*Виконав:\*\* Пилипенко Артемій Валерійович



\*\*Група:\*\* 6.1213-2пі



\*\*Дата виконання:\*\* 22.09.2026





\## Тестовий об’єкт





SauceDemo

https://www.saucedemo.com/





\## Тестове середовище





\- Операційна система: Windows 11

\- Браузер: Opera GX

\- Дата тестування: 22.09.2026





\## Базовий сценарій





За допомогою облікового запису `performance\_glitch\_user` було перевірено швидкість авторизації. За допомогою облікового запису `error\_user` було перевірено процес оформлення замовлення.





\## Виявлені аномалії





№1



Користувач: performance\_glitch\_user



Короткий опис: \[Login] Затримка відкриття Products для performance\_glitch\_user



Severity: Medium



Priority: Medium



Issue : https://github.com/sduvybsygvbygs/software-quality/issues/1#issue-5542072661





№2



Користувач: error\_user



Короткий опис: \[Checkout: Your Information] Поле для вводу прізвища не функціонує під час введення особистих даних.



Severity: Medium



Priority: High



Issue : https://github.com/sduvybsygvbygs/software-quality/issues/2#issue-5542103934





№3



Користувач: error\_user



Короткий опис: \[Checkout: Overview] Кнопка для підтвердження замовлення не функціонує.



Severity: Critical



Priority: High



Issue : https://github.com/sduvybsygvbygs/software-quality/issues/3#issue-5542121163





\## Висновок





У ході виконання лабораторної роботи було проведено аналіз якості вебзастосунку SauceDemo та виконано перевірку його роботи з використанням облікових записів performance\_glitch\_user та error\_user. Під час тестування було виявлено та задокументовано три аномалії різного рівня критичності. Для кожної аномалії визначено Severity та Priority, а також створено відповідний Issue у GitHub із описом проблеми та кроками для її відтворення.

