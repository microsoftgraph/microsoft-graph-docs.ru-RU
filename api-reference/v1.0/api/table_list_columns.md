# <a name="list-columns"></a>Список столбцов

Получение списка объектов tableColumn.
## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуются указанные **области**: 
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables(<id|name>)/columns
GET /workbook/worksheets(<id|name>)/tables(<id|name>)/columns
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Authorization  | Токен носителя.|


## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.
## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [TableColumn](../resources/tablecolumn.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables(<id|name>)/columns
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 126

{
  "value": [
    {
      "id": 99,
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->