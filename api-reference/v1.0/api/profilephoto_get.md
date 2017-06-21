# <a name="get-photo"></a>Получение фотографии

Получение указанного объекта [profilePhoto](../resources/profilephoto.md) или его метаданных (свойств profilePhoto).

Операция GET выполняет поиск указанной фотографии в почтовом ящике пользователя в Exchange Online.

> **Примечание.** Эта операция в версии 1.0 поддерживает только рабочие или учебные почтовые ящики пользователя (не личные).

## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из указанных **областей** (в зависимости от типа фотографии):

*   Фотография профиля любого пользователя в клиенте, в том числе пользователя, вошедшего в систему: *User.ReadBasic.All; User.Read.All; User.ReadWrite.All*.
*   Фотография профиля конкретного пользователя, вошедшего в систему: *User.Read, User.ReadWrite; User.ReadBasic.All; User.Read.All; User.ReadWrite.All*.
* Фотография профиля **группы** - *Group.Read.All; Group.ReadWrite.All*.
* Фотография **контакта** - *Contacts.ReadWrite*.

## <a name="http-request-to-get-the-photo"></a>HTTP-запрос для получения фотографии
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo/$value
GET /users/{id | userPrincipalName}/photo/$value
GET /groups/{id}/photo/$value
GET /me/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contacts/{id}/photo/$value
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="http-request-to-get-the-metadata-of-the-photo"></a>HTTP-запрос для получения метаданных фотографии
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | строка  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Основной текст запросов
Не указывайте основной текст запроса для этого метода.
## <a name="response-for-getting-the-photo"></a>Отклик для запроса на получение фотографии
При успешном выполнении этот метод возвращает код отклика `200 OK` и двоичные данные запрашиваемой фотографии.  Если фотография не существует, операция возвратит отклик `404 Not Found`.
## <a name="response-for-getting-the-metadata-of-the-photo"></a>Отклик для запроса на получение метаданных фотографии
При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [profilePhoto](../resources/profilePhoto.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request-1"></a>Запрос 1
Этот запрос возвращает фотографию пользователя, вошедшего в систему, с максимальным доступным размером.
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a>Отклик 1
Содержит двоичные данные запрошенной фотографии. Код HTTP-отклика: 200.

##### <a name="request-2"></a>Запрос 2
Этот запрос возвращает метаданные фотографии пользователя, выполнившего вход в систему.
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-2"></a>Отклик 2

В данных указанного ниже отклика содержатся метаданные фотографии. Примечание. Показанный здесь объект отклика может быть усечен для краткости.
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

Ниже показаны данные отклика в случае, если фотография пользователя еще не выложена. Примечание. Показанный здесь объект отклика может быть усечен для краткости.

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
