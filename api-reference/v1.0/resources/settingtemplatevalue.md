# <a name="settingtemplatevalue-resource-type"></a>Тип ресурса settingTemplateValue

Представляет определение отдельного параметра шаблона, включая значение по умолчанию для этого параметра, если экземпляр этого параметра не создан.

### <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|defaultValue|String| Значение по умолчанию для параметра. |
|description|String| Описание параметра. |
|name|String| Имя параметра. |
|type|String| Тип параметра. |

### <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->