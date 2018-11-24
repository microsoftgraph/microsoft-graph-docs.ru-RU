# <a name="operationerror-resource-type"></a>Тип ресурса operationError



Описание ошибки в [teamsAsyncOperation](teamsasyncoperation.md).

## <a name="operationerror-properties"></a>operationError свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|code|String (только для чтения)|Код ошибки операции.|
|message|String (только для чтения)|Сообщение об ошибке операции.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
