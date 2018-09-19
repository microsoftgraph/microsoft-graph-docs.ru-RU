# <a name="securityvendorinformation-resource-type"></a>Тип ресурса securityVendorInformation

Содержит сведения о безопасности продуктов и услуг производителя, поставщика и субпоставщика (например, производитель=Майкрософт; поставщик=ATP Защитник Windows; субпоставщик=AppLocker).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|provider *|String|Определенный поставщик (продуктов/услуг - не организация-производитель); например, WindowsDefenderATP.|
|providerVersion|String|Версия поставщика или субпоставщика (при наличии), которая создала оповещение.|
|subProvider|String|Определенный субпоставщик (в разделе статистической обработки поставщика); например, WindowsDefenderATP.SmartScreen.|
|vendor *|String|Имя оповещения производителя (например, Microsoft, Dell, FireEye).|
(\* указывает на обязательный характер.)

## <a name="json-representation"></a>Представление JSON

Далее отображено представление ресурса JSON.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
