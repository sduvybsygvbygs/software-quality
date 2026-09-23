## Test Conditions



- TCND-01 - успішна авторизація валідного користувача;

- TCND-02 - авторизація з неправильним Username;

- TCND-03- авторизація з неправильним Password;

- TCND-04 - авторизація з порожнім Username;

- TCND-05 - авторизація з порожнім Password;

- TCND-06 - авторизація заблокованого користувача.





## Checklist



- \[] Успішна авторизація з валідними даними.

- \[] Відмова в авторизації за неправильним Username.

- \[] Відмова в авторизації з неправильним Password.

- \[] Перевірка порожнього Username.

- \[] Перевірка порожнього Password.

- \[] Відмова в авторизації заблокованого користувача.





### TC-LOGIN-01 - Успішна авторизація standard_user



*Type:* Positive



*Preconditions:*

- відкрита сторінка Login;

- користувач не авторизований.



*Test Data:*

- Username: standard_user

- Password: secret_sauce



*Steps:*

1. У поле Username ввести standard_user
2. У поле Password ввести secret_sauce
3. Натиснути кнопку Login



*Expected Result:*



Після введення standart_user і правильного пароля та натискання Login користувач успішно авторизується.



*Actual Result:*



Після введення standart_user і правильного пароля та натискання Login відкрилася сторінка на Products.



*Result:*



Pass





### TC-LOGIN-02 - Відмова в авторизації standard_user з неправильним паролем



*Type:* Negative



*Preconditions:*

- відкрита сторінка Login;

- користувач не авторизований.



*Test Data:*

- Username: standard_user

- Password: wrong_password



*Steps:*

1. У поле Username ввести standard_user
2. У поле Password ввести wrong_password
3. Натиснути кнопку Login



*Expected Result:*



Після введення standart_user і неправильного пароля та натискання Login авторизацію буде відхилено, а користувач отримає повідомлення "Epic sadface: Username and password do not match any user in this service".



*Actual Result:*



Після введення standart_user і неправильного пароля та натискання Login авторизацію було відхилено, а користувач отримав відповідне повідомлення.



*Result:*



Pass





### TC-LOGIN-03 - Відмова в авторизації locked_out_user



*Type:* Negative



*Preconditions:*

- відкрита сторінка Login;

- користувач не авторизований.



*Test Data:*

- Username:locked\_out\_user

- Password: secret\_sauce



*Steps:*

1. У поле Username ввести standard\_user
2. У поле Password ввести secret\_sauce
3. Натиснути кнопку Login



*Expected Result:*



Після введення locked_out_user і правильного пароля та натискання Login авторизацію буде відхилено а користувач отримає повідомлення "Epic sadface: Sorry, this user has been locked out.".



*Actual Result:*



Після введення locked_out_user і правильного пароля та натискання Login авторизацію було відхилено, а користувач отримав відповідне повідомлення.



*Result:*



Pass

