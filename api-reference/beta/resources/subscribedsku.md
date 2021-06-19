---
title: Тип ресурса subscribedSku
description: Представляет тип SKU с подпиской.
localization_priority: Normal
author: SumitParikh
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 3d41247ebb88e4941556408fe6fbebbabc54ff8d
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030903"
---
# <a name="subscribedsku-resource-type"></a>Тип ресурса subscribedSku

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|capabilityStatus|String| Возможные значения: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`. The capabilityStatus is `Enabled` if the **prepaidUnits** property has at least 1 unit that is **enabled,** and `LockedOut` if the customer cancelled their subscription. |
|consumedUnits|Int32| Количество лицензий, которые были назначены. |
|id|String| Уникальный идентификатор объекта sku, подписка на который выполнена. Key, not nullable. |
|prepaidUnits|[licenseUnitsDetail](licenseunitsdetail.md)| Сведения о количестве и состоянии предварительно оплаченных лицензий. |
|servicePlans|Коллекция [servicePlanInfo](serviceplaninfo.md)| Сведения о планах обслуживания, доступных в отношении SKU. Не является недействительным |
|skuId|Guid| Уникальный идентификатор (GUID) для SKU службы. |
|skuPartNumber|String| Артикул SKU, например: AAD_PREMIUM или RMSBASIC. Чтобы получить список коммерческих подписок, приобретенных организацией, см. в [журнале List subscribedSkus.](../api/subscribedsku-list.md) |

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
<!--
{
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


