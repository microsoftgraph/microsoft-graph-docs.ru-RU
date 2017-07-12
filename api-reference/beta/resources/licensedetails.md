<a id="licensedetails-resource-type" class="xliff"></a>

# Тип ресурса licenseDetails

Содержит сведения о лицензии, назначенной пользователю.

<a id="methods" class="xliff"></a>

## Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление licenseDetails](../api/user_list_licensedetails.md) | Коллекция licenseDetails |Получение списка объектов licenseDetails для пользователя.|

<!--|[Get licenseDetails](../api/licensedetails_get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

<a id="properties" class="xliff"></a>

## Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор объекта сведений о лицензии. Только для чтения, ключевое, не допускает значения null. |
|servicePlans|Коллекция [servicePlanInfo](serviceplaninfo.md)| Сведения о планах обслуживания, назначенных вместе с лицензией. Только для чтения, не допускает значения null. |
|skuId|Guid| Уникальный идентификатор (GUID) для SKU службы. Имеет то же значение, что и свойство skuId в связанном объекте [SubscribedSku](subscribedsku.md). Только для чтения. |
|skuPartNumber|String| Уникальное отображаемое имя SKU. Имеет то же значение, что и свойство skuPartNumber в связанном объекте [SubscribedSku](subscribedsku.md). Пример: AAD_Premium. Только для чтения. |

<a id="relationships" class="xliff"></a>

## Связи
Нет

<a id="json-representation" class="xliff"></a>

## Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->