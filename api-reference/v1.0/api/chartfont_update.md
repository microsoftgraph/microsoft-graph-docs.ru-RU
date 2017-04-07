# <a name="update-chartfont"></a>Обновление объекта ChartFont

Обновление свойств объекта ChartFont.
## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуются указанные **области**: 
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets(<id|name>)/charts(<name>)/axes/valueaxis/format/font
PATCH /workbook/worksheets(<id|name>)/charts(<name>)/axes/seriesaxis/format/font
PATCH /workbook/worksheets(<id|name>)/charts(<name>)/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a>Необязательные заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Authorization  | Токен носителя.|


## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|bold|boolean|Указывает, является ли шрифт полужирным.|
|color|string|HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.|
|italic|boolean|Указывает, применяется ли курсив.|
|name|string|Имя шрифта (например, Calibri)|
|size|Double|Размер шрифта (например, 11)|
|underline|string|Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`.|

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartFont](../resources/chartfont.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets(<id|name>)/charts(<name>)/axes/valueaxis/format/font
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->