---
title: Тип ресурса licenseUnitsDetail
description: Свойство **prepaidUnits** объекта subscribedSku относится к типу **licenseUnitsDetail**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: krbain
ms.openlocfilehash: c241ed81ee7c8b724352c4cac6505595c47c6b7a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029192"
---
# <a name="licenseunitsdetail-resource-type"></a>Тип ресурса licenseUnitsDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Свойство **prepaidUnits** объекта [subscribedSku](subscribedsku.md) относится к типу **licenseUnitsDetail**.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:-------------|:-----|:----------|
|enabled|Int32| Количество включенных единиц. |
|suspended|Int32| Количество приостановленных единиц. |
|warning|Int32| Количество единиц, которые находятся в состоянии предупреждения. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


