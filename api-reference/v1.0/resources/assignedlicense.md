---
title: Тип ресурса assignedLicense
description: Представляет лицензию, назначенную пользователю. Свойство **assignedLicenses** объекта user представляет собой коллекцию объектов **assignedLicense**.
ms.localizationpriority: medium
author: jconley76
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 1aa1dd00d83eb9362b1a13660c12f6109aa80c89
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549542"
---
# <a name="assignedlicense-resource-type"></a>Тип ресурса assignedLicense

Пространство имен: microsoft.graph

Представляет лицензию, назначенную пользователю. Свойство **assignedLicenses** объекта [user](user.md) представляет собой коллекцию объектов **assignedLicense**.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|disabledPlans|Коллекция объектов Guid|Коллекция уникальных идентификаторов отключенных планов.|
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
  "disabledPlans": ["Guid"],
  "skuId": "Guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

