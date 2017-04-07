# <a name="alternativesecurityid-resource-type"></a>Тип ресурса alternativeSecurityId

Содержит альтернативный ИД безопасности, связанный с устройством. Свойство **alternativeSecurityIds** объекта [Device](device.md) представляет собой коллекцию объектов **alternativeSecurityId**.

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|identityProvider|String|            |
|key|Двоичный|            |
|type|Int32|            |


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "identityProvider": "string",
  "key": "binary",
  "type": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alternativeSecurityId resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
