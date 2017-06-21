# <a name="page-copytosection"></a>page: copyToSection
Копирование страницы в определенный раздел.

Для операций Copy необходимо использовать модель асинхронного вызова.  То есть сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.

## <a name="prerequisites"></a>Необходимые условия
Для выполнения этого API требуется одно из следующих **разрешений**:   

Notes.Create, Notes.ReadWrite или Notes.ReadWrite.All.  

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | строка  | Bearer {токен}. Обязательный. |
| Content-Type | строка | `application/json` |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите объект JSON, который содержит параметры, требуемые операцией.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|groupId|String|Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.|
|id|String|Обязательный. Идентификатор целевого раздела.|


## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation_get.md), опросите конечную точку Operation-Location.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <a name="response"></a>Отклик
Ниже приведен пример ответа.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->