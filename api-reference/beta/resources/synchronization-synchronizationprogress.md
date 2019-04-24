---
title: Тип ресурса Синчронизатионпрогресс
description: Представляет ход выполнения Синчронизатионжоб в сторону завершения.
localization_priority: Normal
ms.openlocfilehash: b22bd95f54a9f268524dc98a8d3df94fcc14f773
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453959"
---
# <a name="synchronizationprogress-resource-type"></a>Тип ресурса Синчронизатионпрогресс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ход выполнения [синчронизатионжоб](synchronization-synchronizationjob.md) в сторону завершения.

## <a name="properties"></a>Свойства

| Свойство                              | Тип      | Описание    |
|:--------------------------------------|:----------|:---------------|
|Комплетедунитс|Int32|Числитель коэффициента выполнения; количество единиц изменений, которые уже обработаны.|
|Прогрессобсерватиондатетиме|DateTimeOffset|Время отслеживания хода выполнения как смещение в минутах от времени в формате UTC.|
|Тоталунитс|Int32|Знаменатель коэффициента выполнения; количество единиц изменений, которые необходимо обработать для выполнения синхронизации.|
|продукции|Строка|Необязательное описание единиц измерения.|

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
