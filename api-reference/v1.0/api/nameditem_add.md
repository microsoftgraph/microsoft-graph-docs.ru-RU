# <a name="add-named-item"></a>Add Named Item

Добавляет новое имя в определенную коллекцию, используя языковой стандарт пользователя для формулы.

## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из указанных **областей**:

  * Files.ReadWrite
  * Sites.Read.All
  
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {code}|


## <a name="request-body"></a>Тело запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр       | Тип    |Описание|
|:---------------|:--------|:----------|
|name|строка|Имя именованного элемента.|
|ссылка|string|Формула или диапазон, на которые будет ссылаться имя.|
|примечание|string|Комментарий, связанный с именованным элементом|

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200, OK` и объект [NamedItem](../resources/NamedItem.md) в тексте отклика.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "myRange",
  "reference": "=A10+B10",
  "comment": "Comment for the named item"
}
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "name": "myRange",
  "comment": "Sample range",
  "scope": "Workbook",
  "type": "String",
  "visible": true,
  "value": "=A10+B10"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
