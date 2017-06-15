# <a name="get-drive"></a>Получение доступа к ресурсу Drive

Получение свойств и отношений ресурса [Drive](../resources/drive.md). Drive — это контейнер верхнего уровня для файловой системы. API Graph позволяет получить доступ к ресурсу Drive для OneDrive, OneDrive для бизнеса и библиотек документов SharePoint.

## <a name="prerequisites"></a>Необходимые условия

Для применения этого API требуется одна из указанных **областей**:

* Files.Read
* Files.ReadWrite
* Sites.Read.All

## <a name="get-a-users-onedrive"></a>Получение доступа к OneDrive пользователя

Чтобы получить доступ к хранилищу пользователя OneDrive или OneDrive для бизнеса, ваше приложение должно запросить отношение **drive** для ресурса [User](../resources/user.md).

### <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive
GET /users/{idOrUserPrincipalName}/drive
```

## <a name="get-the-document-library-associated-with-a-group"></a>Получение библиотеки документов, связанной с группой

Для доступа к библиотеке документов [группы](../resources/group.md) по умолчанию приложение запрашивает отношение **drive** для объекта Group.

### <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{idOrUserPrincipalName}/drive
```


## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.

## <a name="request-body"></a>Тело запроса

Не указывайте тело запроса для этого метода.

## <a name="response"></a>Ответ

В случае успеха этот метод возвращает код ответа `200 OK` и ресурс [Drive](../resources/drive.md) в теле ответа.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса для получения сведений о хранилище OneDrive для бизнеса или OneDrive пользователя после входа.

<!-- {
  "blockType": "request",
  "name": "get_drive"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive
```

##### <a name="response"></a>Ответ

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get Drive"
}-->
