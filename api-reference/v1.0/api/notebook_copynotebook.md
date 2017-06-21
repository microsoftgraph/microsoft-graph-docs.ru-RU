# <a name="notebook-copynotebook"></a>notebook: copyNotebook
Копирование записной книжки в папку Notebooks в целевой библиотеке документов. Если такой папки нет, она будет создана.

Для операций Copy необходимо использовать модель асинхронного вызова.  То есть сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.

## <a name="prerequisites"></a>Необходимые условия
Для выполнения этого API требуется одно из следующих **разрешений**:   

Notes.Create, Notes.ReadWrite или Notes.ReadWrite.All. 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | строка  | Bearer {токен}. Обязательный. |
| Content-Type | строка | `application/json` |

## <a name="request-body"></a>Текст запроса
В теле запроса укажите объект JSON, который содержит параметры, требуемые операцией. Если тело не нужно, можно отправить пустое тело.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|groupId|String|Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.|
|renameAs|String|Имя копии. По умолчанию используется имя существующего элемента. |


## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteOperation_get.md), опросите конечную точку Operation-Location.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
