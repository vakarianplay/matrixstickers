# matrixstickers
Fork maunium/stickerpicker repo

-----------------------------------------

# Подключение менеджера стикеров к клиенту Element

* Заходим в настройки *любого* чата

 > ![Image alt](https://github.com/vakarianplay/matrixstickers/blob/main/manualpic/1-1.png)


* Заходим в пункт **"подробности"** и открываем **"инструменты разработчика"**

 > ![Image alt](https://github.com/vakarianplay/matrixstickers/blob/main/manualpic/2.png)
 
 
* Нажимаем на кнопку **"Отправка параметров учетной записи"**

 > ![Image alt](https://github.com/vakarianplay/matrixstickers/blob/main/manualpic/3.png)


* Тип события указываем `m.widgets`
* Очищаем поле "содержимое события", вставляем следующий код и нажимаем **"отправить"**
  ```json
  {
    "stickerpicker": {
        "content": {
            "type": "m.stickerpicker",
            "url": "https://vakarian.website/matrixstickers/?theme=$theme",
            "name": "Stickerpicker",
            "data": {}
        },
        "sender": "@you:matrix.server.name",
        "state_key": "stickerpicker",
        "type": "m.widget",
        "id": "stickerpicker"
    }
  }


 > ![Image alt](https://github.com/vakarianplay/matrixstickers/blob/main/manualpic/4.png)


* После получения сообщения **"событие успешно отправлено"** закрываем это окно.

 > ![Image alt](https://github.com/vakarianplay/matrixstickers/blob/main/manualpic/5.png)


# Стикеры готовы к использованию
