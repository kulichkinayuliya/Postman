# 📝 Postman
Рабоче пространство в [Postman](https://www.postman.com/satellite-cosmologist-1082208/workspace/test-workspace/collection/30288313-654ce6f1-ddbd-4434-89ee-18ca148b11f0)
---

## ✏️ Задание 1
### Условие: 
1. Получите список пользователей. Каким запросом получили список пользователей? Какой статус ответа получили? Что содержится в теле ответа? Сделайте скриншот

### ✔️ Решение:
GET-запрос. Статус ответа - 200 ОК. В теле ответа содежится информация о пользователях (id, name, email, gender, status).

![](https://github.com/kulichkinayuliya/Postman/blob/main/file/Postman_AiXovVvNJL.png)

2. Модифицируйте запрос и получите страницу 12. Что содержится в теле ответа? Сделайте скриншот.

### ✔️ Решение:
В теле ответа содержится информация о пользователях на странице 12.

![](https://github.com/kulichkinayuliya/Postman/blob/main/file/Postman_ywUtsRnKmn.png)

3. Сделайте post запрос для получения пользователя с пустым телом запроса. Какой ответ пришел и почему? Сделайте
скриншот.

### ✔️ Решение:
Тело ответа: Поля не могут быть пустыми. Статус код - 422. POST-запросы направлены надобавление информации в ресурс, следовательно должны содержать тело запроса.

![](https://github.com/kulichkinayuliya/Postman/blob/main/file/Postman_XxFSRtrpxF.png)

4. Напишите запрос для создания пользователя, используя метод raw => json. Какой ответ пришел? Сделайте скриншот

### ✔️ Решение:
Пользователь создан. Указанный логин при добавлении пользователя автоматически меняется на системный. Без логина пользователя добавить нельзя, получаем ошибку: "Error occurred while parsing request parameters". Статус код - 201.

![](https://github.com/kulichkinayuliya/Postman/blob/main/file/Postman_QsPEjI4KYA.png)

5. Напишите запрос, возвращающий в ответе запись о созданном пользователе. Сделайте скриншот.
   
### ✔️ Решение:
![](https://github.com/kulichkinayuliya/Postman/blob/main/file/Postman_4WwUGWrkB6.png)

6. Создайте еще несколько пользователей с одинаковыми значениями “name”, но разными email. Получите список всех только что созданных пользователей. Сделайте скриншот.

### ✔️ Решение:
![](https://github.com/kulichkinayuliya/Postman/blob/main/file/Postman_G25i1kNwwY.png)

7. Напишите запрос с методом put на изменение email и name на другое значение. Проверьте изменение get запросом. Сделайте скриншот.

### ✔️ Решение:
![](https://github.com/kulichkinayuliya/Postman/blob/main/file/Postman_pzBcK4prmi.png)

8. Чем отличаются запросы put и patch? Напишите запрос с методом patch для корректировки полей status и email. Сделайте скриншот. В чем отличие полученного результата, от результата запроса из п.7?

### ✔️ Решение:

PATCH используется для частичного изменения ресурса. PUT создает новый ресурс или заменяет представление целевого ресурса, данными представленными в теле запроса. 

В целом методы PATCH и PUT работают одинаково. Отличия возникают только тогда, когда мы хотим изменить одно из полей. Например, у нас хранится информация об имени и фамилии пользователя. Написав запрос на изменение только имени методом PUT, у нас изменится поле имя, а поле фамилия очистится, так как мы его не передали. Если же написать запрос на изменение имени методом PATCH, поле имя у нас изменится, а поле фамилия будет не затронуто.

### ✔️ Решение:
![](https://github.com/kulichkinayuliya/Postman/blob/main/file/Postman_oWWIvEP3WV.png)

9. Удалите пользователя, созданного в п.4. Что содержится в теле ответа? Сделайте скриншот. Выполните get запрос удаленного пользователя. Сделайте скриншот.

### ✔️ Решение:
![](https://github.com/kulichkinayuliya/Postman/blob/main/file/Postman_s8Qk891G1I.png)
![](https://github.com/kulichkinayuliya/Postman/blob/main/file/Postman_5tvv0TN5PH.png)








