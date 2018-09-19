# <a name="cloudappsecuritystate-resource-type"></a>тип ресурса cloudAppSecurityState

Содержит информацию о состоянии облачного приложения (destinationServiceName, destinationServiceIp).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|destinationServiceIp|Строка|Конечный IP-адрес подключения к облачному приложению / службе.|
|destinationServiceName|Строка|Имя облачного приложения / службы (например «Salesforce», «DropBox» и т.д.).|
|riskScore|Строка|Указанная поставщиком / рассчитанная оценка рисков для облачного приложения / службы. Рекомендуемый диапазон значений: от 0 до 1, что соответствует величине в процентах.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->