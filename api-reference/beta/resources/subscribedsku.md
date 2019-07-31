---
title: Тип ресурса subscribedSku
description: " Создание, обновление и удаление не поддерживаются. Выражения фильтра запросов не поддерживаются. Наследуется от directoryObject."
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e57ff1e59c7caf5b29e582b7381492a7eee5b4c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964833"
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
