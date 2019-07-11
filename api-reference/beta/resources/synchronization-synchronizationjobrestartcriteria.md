---
title: Тип ресурса Синчронизатионжобрестарткритериа
description: 'Определяет область действия [синчронизатионжоб: Restart](../api/synchronization_synchronizationjob_restart.md) .'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fda28a84f568b9d535a06226397375f3fa8e444a
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620726"
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
