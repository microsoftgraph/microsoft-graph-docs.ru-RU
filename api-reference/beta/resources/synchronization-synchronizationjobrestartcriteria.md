---
title: Тип ресурса Синчронизатионжобрестарткритериа
description: 'Определяет область действия Синчронизатионжоб: restart.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 82d671f411725a1e6537580205c7298cf887e3a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023844"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>Тип ресурса Синчронизатионжобрестарткритериа

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет область действия [синчронизатионжоб: Restart](../api/synchronization-synchronizationjob-restart.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ресетскопе|String| Разделенная запятыми комбинация следующих значений: `Full` ,,, `QuarantineState` `Watermark` `Escrows` , `ConnectorDataStore` . Используйте `Full` , если вы хотите использовать все параметры.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
    "criteria": {
        "resetScope": "String"
    }
}


```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


