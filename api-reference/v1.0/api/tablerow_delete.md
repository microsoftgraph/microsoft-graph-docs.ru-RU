# <a name="tablerow-delete"></a>TableRow: delete

Удаляет строку из таблицы.
## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуются указанные **области**: 

    * Files.ReadWrite.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows(<index>)/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)/delete

```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |


## <a name="request-body"></a>Текст запроса

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)/delete
```

##### <a name="response"></a>Отклик
Ниже приведен пример ответа. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->