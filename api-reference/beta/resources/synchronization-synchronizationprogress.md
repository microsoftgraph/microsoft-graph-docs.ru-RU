---
title: Тип ресурса Синчронизатионпрогресс
description: Представляет ход выполнения Синчронизатионжоб в сторону завершения.
localization_priority: Normal
ms.openlocfilehash: d05193c7c242dc3f890aba6f4fcec5a8badc087f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340017"
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
|продукции|String|Необязательное описание единиц измерения.|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationProgress"
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
  "suppressions": []
}
-->
