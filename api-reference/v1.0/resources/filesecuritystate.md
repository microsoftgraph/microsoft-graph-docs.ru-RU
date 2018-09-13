# <a name="filesecuritystate-resource-type"></a>Тип ресурса fileSecurityState

Содержит информацию о файле (не процессе), связанную с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|Сложный тип, содержащий хэши файлов (криптографические и чувствительные к расположению).|
|name|String|Имя файла (без пути).|
|path|String|Полный путь к файлу или объекту imageFile.|
|riskScore|String|Сгенерированная/расчитанная поставщиком оценка риска для файла оповещений. Рекомендуемый диапазон значений: от 0 до 1, что соответствует величине в процентах.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->