Итак дошли руки написать мини-руководство. Сразу хочу предупредить, что лучше всего проверку данных делать в облаке - это безопасно,  но в даном случае реализован простой вариант с проверкой внутри приложения, используя package:crypto

Делайте по шагам:
1. Создать DataType currentUser, поля в нем на фото: (нужен чтобы распарсить данные, которые отдаст Телеграм)
2. Добавить зависимость crypto: ^3.0.5
3. 2 файла слева, их нужно скопировать и добавить в ваш FF проект.
4. Добавить в разделе Веб в заголовок :
<script src="https://telegram.org/js/telegram-web-app.js"></script>
<script src="https://unpkg.com/@tonconnect/sdk@latest/dist/tonconnect.umd.min.js"></script>


![image](https://github.com/user-attachments/assets/11c53af8-202a-4f7c-a773-8dacc977f77a)



 ![image](https://github.com/user-attachments/assets/5f544bef-0fae-43ee-98e3-dbf0003d5173)

 5. Первым на PageLoad ставим tgInitData. Когда телеграм вернул данные - проверяем через второй экшен и обновите документ в БД, те поля что вам нужно!

 Все готово! Наслаждайтесь :) Если нужна помощь я всегда на связи! https://t.me/bohvik
 
 Угостить меня кофе https://www.tinkoff.ru/rm/r_udcxElYlNk.gNwrTuckdF/VH0oR18434


