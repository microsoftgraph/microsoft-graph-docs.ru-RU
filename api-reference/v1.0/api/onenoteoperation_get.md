# <a name="get-onenoteoperation"></a>Получение onenoteOperation

Получение сведений о состоянии операции OneNote, выполняющейся в течение длительного времени. Применяется к операциям, возвращающим заголовок **Operation-Location** в отклике, например `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.   

Вы можете опрашивать конечную точку Operation-Location, пока свойство `status` не возвратит значение `completed` или `failed`. 

Если операция имеет состояние `completed`, свойство `resourceLocation` содержит URI конечной точки ресурса. 

Если операция имеет состояние `failed`, свойства `@api.diagnostics` и error предоставляют данные об ошибке.

## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из следующих **областей**:  

Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All или Notes.ReadWrite.All.  

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Нет.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | `Bearer <token>` (приложению предоставляется допустимый токен OAuth на основании учетных данных пользователя и пользователя c разрешенным доступом) |
| Accept | string | `application/json` | 

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.
## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [onenoteOperation](../resources/onenoteoperation.md) в теле отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/operations/{id}
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "id": "id-value",
  "status": "status-value",
  "createdDateTime": "2016-10-19T10:37:00Z",
  "lastActionDateTime": "2016-10-19T10:37:00Z",
  "resourceLocation": "resourceLocation-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
