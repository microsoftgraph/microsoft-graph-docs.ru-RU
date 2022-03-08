---
title: Тип ресурса subscribedSku
description: Содержит сведения о SKU службы, на которую компания подписана.
ms.localizationpriority: medium
author: SumitParikh
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ed4a509a0f222e0853848b99caf0bc4ddee31685
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333136"
---
# <a name="subscribedsku-resource-type"></a>Тип ресурса subscribedSku

Пространство имен: microsoft.graph

Содержит сведения о SKU службы, на которую компания подписана.

Только операция чтения поддерживается в поддерживаемых skUs; создание, обновление и удаление не поддерживаются. Выражения фильтра запросов не поддерживаются. Наследуется от [directoryObject](directoryobject.md).

## <a name="methods"></a>Методы
| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта subscribedSku](../api/subscribedsku-get.md) | [subscribedSku](subscribedsku.md) |Получение определенной коммерческой подписки, приобретенной организацией.|
|[Список subscribedsku](../api/subscribedsku-list.md) | Коллекция объектов [subscribedSku](subscribedsku.md) |Получение списка коммерческих подписок, приобретенных организацией.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appliesTo|String| Например, User или Company. |
|capabilityStatus|String|  Возможные значения: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`. The capabilityStatus is `Enabled` if the **prepaidUnits** property has at least 1 unit that is **enabled**, and `LockedOut` if the customer cancelled their subscription. |
|consumedUnits|Int32| Количество лицензий, которые были назначены. |
|id|Строка| Уникальный идентификатор объекта sku, подписка на который выполнена. Key, not nullable. |
|prepaidUnits|[licenseUnitsDetail](licenseunitsdetail.md)| Сведения о количестве и состоянии предварительно оплаченных лицензий. |
|servicePlans|Коллекция [servicePlanInfo](serviceplaninfo.md)| Сведения о планах обслуживания, доступных в отношении SKU. Не является недействительным |
|skuId|Guid| Уникальный идентификатор (GUID) для SKU службы. |
|skuPartNumber|String| Артикул SKU, например: AAD_PREMIUM или RMSBASIC. Чтобы получить список коммерческих подписок, приобретенных организацией, см. в [примере List subscribedSkus](../api/subscribedsku-list.md).|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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
  "appliesTo": "String",
  "capabilityStatus": "String",
  "consumedUnits": 1024,
  "id": "String (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

## <a name="see-also"></a>См. также

+ [Названия продуктов и идентификаторы планов служб для лицензирования](/azure/active-directory/enterprise-users/licensing-service-plan-reference)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

