---
title: Тип ресурса synchronizationProgress
description: Представляет ход выполнения synchronizationJob к завершению.
localization_priority: Normal
ms.openlocfilehash: b22bd95f54a9f268524dc98a8d3df94fcc14f773
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640072"
---
# <a name="synchronizationprogress-resource-type"></a>Тип ресурса synchronizationProgress

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ход выполнения [synchronizationJob](synchronization-synchronizationjob.md) к завершению.

## <a name="properties"></a>Свойства

| Свойство                              | Тип      | Описание    |
|:--------------------------------------|:----------|:---------------|
|completedUnits|Int32|Числитель соотношение хода выполнения; Количество единиц уже обработки изменений.|
|progressObservationDateTime|DateTimeOffset|Время наблюдения хода выполнения как смещение в минутах от времени UTC.|
|totalUnits|Int32|Делителя соотношение хода выполнения; Количество единиц изменения обработки для выполнения синхронизации.|
|единицы|String|Необязательное описание единицы измерения.|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
}-->

```json
{
  "completedUnits": 1025,
  "progressObservationDateTime": "2017-10-10T17:00:00Z",
  "totalUnits": 3024,
  "units": "pages"
}

```

<!-- uuid: 15571993-7e2f-4842-84d5-01ceb67cdc05
20185-08-14 22:30:00 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationprogress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
