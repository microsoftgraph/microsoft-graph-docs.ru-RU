# <a name="subscribedsku-resource-type"></a>Тип ресурса subscribedSku

Содержит сведения о сервисе SKU, на который подписана компания.

В подписанных SKU поддерживается только операция чтения. Создание, обновление и удаление не поддерживаются. Выражения фильтра запроса не поддерживаются. Наследуется от [directoryObject](directoryobject.md).

## <a name="methods"></a>Методы
| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта subscribedSku](../api/subscribedsku_get.md) | [subscribedSku](subscribedsku.md) |Чтение свойств и связей объекта subscribedSku.|
|[Список  subscribedsku](../api/subscribedsku_list.md) | Коллекция [subscribedSku](subscribedsku.md) |Получение списка коммерческих подписок, приобретенных организацией.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appliesTo|String (строка)| Например, User или Company. |
|capabilityStatus|String (строка)| Например, Enabled. |
|consumedUnits|Int32| Количество лицензий, которые были назначены. |
|id|String (строка)| Уникальный идентификатор объекта sku, подписка на который выполнена. Ключ, значение NULL не допускается. |
|prepaidUnits|[licenseUnitsDetail](licenseunitsdetail.md)| Сведения о количестве и состоянии предварительно оплаченных лицензий. |
|servicePlans|Коллекция [servicePlanInfo](serviceplaninfo.md)| Сведения о планах обслуживания, доступных в отношении SKU. Значение NULL не допускается |
|skuId|Guid| Уникальный идентификатор (GUID) для SKU службы. |
|skuPartNumber|String (строка)| Артикул SKU, например: AAD_PREMIUM или RMSBASIC. |

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscribedSku",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
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
