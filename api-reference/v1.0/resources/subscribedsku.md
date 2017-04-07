# <a name="subscribedsku-resource-type"></a>Тип ресурса subscribedSku

Содержит сведения о SKU службы, на которую компания подписана.

В случае SKU службы, на которую выполнена подписка, поддерживаются только операции чтения. Создание, обновление и удаление не поддерживаются. Выражения фильтра запроса не поддерживаются.

Наследуется от [directoryObject](directoryobject.md).


## <a name="methods"></a>Методы
| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта subscribedSku](../api/subscribedsku_get.md) | [subscribedSku](subscribedsku.md) |Считывает свойства объекта subscribedSku.|

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|capabilityStatus|String|Например, Enabled, LockedOut и Suspended.|
|consumedUnits|Int32|Количество лицензий, которые были назначены.|
|id|String|Уникальный идентификатор объекта sku, подписка на который выполнена. Ключ. Только для чтения.|
|prepaidUnits|[licenseUnitsDetail](licenseunitsdetail.md)|Сведения о количестве и состоянии предварительно оплаченных лицензий.|
|servicePlans|Коллекция [servicePlanInfo](serviceplaninfo.md)|Сведения о планах обслуживания, доступных в отношении SKU.|
|skuId|Guid|Уникальный идентификатор (GUID) для SKU службы.|
|skuPartNumber|String|Артикул SKU, например: AAD_PREMIUM или RMSBASIC.|
|appliesTo|String|Например, User или Company.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subscribedSku"
}-->

```json
{
  "appliesTo": "string",
  "capabilityStatus": "string",
  "consumedUnits": 1024,
  "id": "string (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "guid",
  "skuPartNumber": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
