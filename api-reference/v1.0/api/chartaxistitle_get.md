# <a name="get-chartaxistitle"></a>Получение объекта ChartAxisTitle

Получение свойств и связей объекта ChartAxisTitle.
## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуются указанные **области**: 
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets(<id|name>)/charts(<name>)/axes/valueaxis/title
GET /workbook/worksheets(<id|name>)/charts(<name>)/axes/seriesaxis/title
GET /workbook/worksheets(<id|name>)/charts(<name>)/axes/categoryaxis/title
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
В случае успеха этот метод возвращает код отклика `200 OK` и объект [ChartAxisTitle](../resources/chartaxistitle.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_chartaxistitle"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets(<id|name>)/charts(<name>)/axes/valueaxis/title
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartAxisTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->