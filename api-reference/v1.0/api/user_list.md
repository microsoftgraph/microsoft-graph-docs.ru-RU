# <a name="list-users"></a>Список пользователей

Получение списка объектов пользователей.

> Примечание. В списке пользователей возвращается только стандартный набор свойств (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). С помощью `$select` можно получить остальные свойства и связи объекта [user](../resources/user.md). Однако только следующие свойства можно выбрать для отдельных пользователей (например, /v1.0/me?$select=aboutMe), не для коллекции пользователей (например, /v1.0/users?$select=aboutMe):
>* aboutMe
>* birthday
>* hireDate
>* interests
>* mySite
>* pastProjects
>* preferredName
>* responsibilities
>* schools
>* skills
>* mailboxSettings

## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуется одна из указанных **областей**: *User.ReadBasic.All; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /users
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение|
|:-----------|:------|
| Авторизация  | Bearer <token>. Обязательный параметр.  |
| Content-Type   | application/json | 

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.
## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
