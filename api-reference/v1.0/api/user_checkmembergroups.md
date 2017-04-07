# <a name="checkmembergroups"></a>checkMemberGroups
Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых указанный пользователь состоит напрямую или транзитивно. 

В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, членство в группе Office 365 всегда непосредственное. 

## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из указанных **областей**: *User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer <token>. Обязательный параметр.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Тело запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр       | Тип    |Описание|
|:---------------|:--------|:----------|
|groupIds|String|Массив идентификаторов групп|

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200, OK` и объект коллекции String в тексте отклика.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
