---
title: Тип ресурса Синчронизатионжобрестарткритериа
description: 'Определяет область действия [синчронизатионжоб: Restart](../api/synchronization_synchronizationjob_restart.md) .'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8fb363b74f1daff678d0751aca4a9033b01d9832
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964657"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>Тип ресурса Синчронизатионжобрестарткритериа

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет область действия [синчронизатионжоб: Restart](../api/synchronization-synchronizationjob-restart.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Ресетскопе|String| Разделенная запятыми комбинация следующих значений: `Full`, `QuarantineState` `Watermark`,, `Escrows`, `ConnectorDataStore`. Используйте `Full` , если вы хотите использовать все параметры.|

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
  "resetScope": "String"
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
