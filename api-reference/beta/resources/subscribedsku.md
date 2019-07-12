---
title: Тип ресурса subscribedSku
description: " Создание, обновление и удаление не поддерживаются. Выражения фильтра запросов не поддерживаются. Наследуется от directoryObject."
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c2bca99fed2b8c5328c2f2cf1ac3bf938ddcfcaa
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2019
ms.locfileid: "35639026"
---
# <a name="subscribedsku-resource-type"></a>Тип ресурса subscribedSku

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

На подписанных SKU поддерживаются только операции чтения; Создание, обновление и удаление не поддерживаются. Выражения фильтра запросов не поддерживаются. Наследуется от [directoryObject](directoryobject.md).


## <a name="methods"></a>Методы
| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта subscribedSku](../api/subscribedsku-get.md) | [subscribedSku](subscribedsku.md) |Получение конкретной коммерческой подписки, приобретенной Организацией.|
|[Список subscribedsku](../api/subscribedsku-list.md) | Коллекция объектов [subscribedSku](subscribedsku.md) |Получение списка коммерческих подписок, приобретенных Организацией.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Тег|String| Например, User или Company. |
|Капабилитистатус|String| Пример: "Enabled". |
|consumedUnits|Int32| Количество лицензий, которые были назначены. |
|id|String| Уникальный идентификатор объекта sku, подписка на который выполнена. Key, не допускающая значение null. |
|Препаидунитс|[licenseUnitsDetail](licenseunitsdetail.md)| Сведения о количестве и состоянии предварительно оплаченных лицензий. |
|Сервицепланс|Коллекция [servicePlanInfo](serviceplaninfo.md)| Сведения о планах обслуживания, доступных в отношении SKU. Не допускает значение null |
|skuId|Guid| Уникальный идентификатор (GUID) для SKU службы. |
|Скупартнумбер|String| Артикул SKU, например: AAD_PREMIUM или RMSBASIC. |

## <a name="relationships"></a>Отношения
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
