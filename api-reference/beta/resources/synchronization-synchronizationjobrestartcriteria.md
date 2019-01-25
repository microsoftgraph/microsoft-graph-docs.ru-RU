---
title: Тип ресурса synchronizationJobRestartCriteria
description: 'Определяет область [synchronizationJob: перезапустите](../api/synchronization_synchronizationjob_restart.md) действие.'
localization_priority: Normal
ms.openlocfilehash: 1e6ac952808f80d191fc93e9a804411ec4459d4c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512642"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>Тип ресурса synchronizationJobRestartCriteria

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет область [synchronizationJob: перезапустите](../api/synchronization_synchronizationjob_restart.md) действие.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|resetScope|String| Разделенный запятыми сочетание следующих значений: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`. Использование `Full` Если вы хотите, чтобы все параметры.|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjobrestartcriteria.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
