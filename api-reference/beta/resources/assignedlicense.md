---
title: Тип ресурса assignedLicense
description: Представляет лицензию, назначенную пользователю. Свойство **assignedLicenses** объекта user представляет собой коллекцию объектов **assignedLicense**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b7d529b62155493655ceccb4db594a6d560ccf84
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508214"
---
# <a name="assignedlicense-resource-type"></a>Тип ресурса assignedLicense

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет лицензию, назначенную пользователю. Свойство **assignedLicenses** объекта [user](user.md) представляет собой коллекцию объектов **assignedLicense**.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|дисабледпланс|Коллекция объектов Guid|Коллекция уникальных идентификаторов отключенных планов.|
|skuId|Guid|Уникальный идентификатор SKU.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
