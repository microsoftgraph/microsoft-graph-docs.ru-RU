---
title: Тип ресурса synchronizationJobRestartCriteria
description: 'Определяет область действия synchronizationJob: действие перезапуска.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: ef15c9322c553d0eedb977c3f01ed5de2823e844
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136509"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>Тип ресурса synchronizationJobRestartCriteria

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет область действия [synchronizationJob: действие перезапуска.](../api/synchronization-synchronizationjob-restart.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|resetScope|Строка| Сочетание следующих значений, разделенных запятой: `Full` , `QuarantineState` , , `Watermark` `Escrows` `ConnectorDataStore` . Используйте, `Full` если вам нужны все параметры.|

## <a name="json-representation"></a>Представление в формате JSON

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


