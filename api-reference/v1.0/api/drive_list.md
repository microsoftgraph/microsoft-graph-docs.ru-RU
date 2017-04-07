# <a name="list-available-drives"></a>Список доступных дисков

Получение списка ресурсов [Drive](../resources/drive.md), доступных целевому объекту [User](../resources/user.md) или [Group](../resources/group.md). Приложение также может запросить набор библиотек документов на корневом сайте SharePoint.
## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуется одна из указанных **областей**:

  * Files.Read
  * Files.ReadWrite
  * Sites.Read.All

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /drives
GET /me/drives
GET /groups/{id}/drives
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Drive](../resources/drive.md) в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос
Ниже приведен пример запроса на получение списка дисков пользователя.

<!-- {
  "blockType": "request",
  "name": "get_drives"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drives
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.drive",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 579

{
  "value": [
    {
      "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
      "driveType": "business",    
      "owner": {
          "user": {
              "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
              "displayName": "Ryan Gregg"
          }
      },
      "quota": {
          "deleted": 256938,
          "remaining": 1099447353539,
          "state": "normal",
          "total": 1099511627776
      }
    }
  ]
}
```

## <a name="remarks"></a>Заметки

У большинства пользователей есть только ресурс Drive. Для групп и некоторых пользователей может быть доступно несколько дисков.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/List Drives"
}-->
