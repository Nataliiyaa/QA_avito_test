1. Несоответствие swagger и postman_collection при ошибке 404
   Ожидаемый результат: тела ответов совпадают в swagger и postman_collection
   Фактический результат: в swagger тело ответа: {}; в postman_collection тело ответа:
   {
      "result": "laborum",
      "status": "cillum enim eiusmod"
    }
   <img width="357" height="198" alt="image" src="https://github.com/user-attachments/assets/74aab499-fe34-4811-b5ff-a55375ab7203" />
   <img width="330" height="96" alt="image" src="https://github.com/user-attachments/assets/93a1cecd-5506-4ab5-8202-5b143c28c2e7" />

2. Карточка создаётся, если лайков больше, чем просмотров
   Шаги: Создать карточку, где лайков больше, чем просмотров
   Ожидаемый результат: ошибка, такое невозможно, так как это нелогично
   Фактический результат: карточка успешно создаётся

3. тело ответа пр 200 коде в ручке POST/api/1/item несоответсвует документации
   Шаги: отправить успешный запрос POST/api/1/item на создание объявления и получить тело ответа
   Ожидаемый результат: тело ответа выглядит так:
   <img width="349" height="353" alt="image" src="https://github.com/user-attachments/assets/cacf1307-4a19-412d-bd29-dde14c8f13d6" />
   Фактический результат: тело ответа выглядит так:
   <img width="571" height="76" alt="image" src="https://github.com/user-attachments/assets/1ffee825-2741-4804-b510-96ec9a76a633" />

4. Объявление создается, если отсутствует цена
   Шаги: создать объявление без поля price
   Ожидаемый результат: статус 400, сообщение "поле price обязательно"
   Фактический результат: объявление успешно создано

5. При запросе GET/api/1/item/ статус код 404, а в теле ответа code: 400
   Шаги: отправить запрос GET/api/1/item/
   Ожидаемый результат: статус код 404 и в теле ответа также code: 404
   Фактический результат: статус код 404, а тело ответа выглядит так:
   <img width="391" height="89" alt="image" src="https://github.com/user-attachments/assets/f96257a2-660d-492c-b567-0eec8ce17837" />

6. При При запросе GET/api/1/item/ статус код 400, а не 404
   Шаги: отправить запрос GET/api/1/item/1
   Ожидаемый результат: статус код 404
   Фактический результат: статус код 400

7. При ошибке 404 тело ответа несоответствует документации
   Шаги: отправить запрос и получить ошибку 404
   Ожидаемый результат:
   <img width="293" height="86" alt="image" src="https://github.com/user-attachments/assets/2cee90d8-34c3-45b9-a7f6-405ea3815e2e" />
   Фактический результат:
   <img width="425" height="94" alt="image" src="https://github.com/user-attachments/assets/66125b11-5d29-473f-9195-8f9f339f4f18" />







