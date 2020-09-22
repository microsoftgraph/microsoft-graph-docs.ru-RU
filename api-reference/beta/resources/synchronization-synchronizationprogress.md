---
title: Тип ресурса Синчронизатионпрогресс
description: Представляет ход выполнения Синчронизатионжоб в сторону завершения.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5040cb32b664497f2cbed9dc9ca77ce2a2a54ee7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023830"
---
# <a name="synchronizationprogress-resource-type"></a>Тип ресурса Синчронизатионпрогресс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ход выполнения [синчронизатионжоб](synchronization-synchronizationjob.md) в сторону завершения.

## <a name="properties"></a>Свойства

| Свойство                              | Тип      | Описание    |
|:--------------------------------------|:----------|:---------------|
|комплетедунитс|Int32|Числитель коэффициента выполнения; количество единиц изменений, которые уже обработаны.|
|прогрессобсерватиондатетиме|DateTimeOffset|Время отслеживания хода выполнения как смещение в минутах от времени в формате UTC.|
|тоталунитс|Int32|Знаменатель коэффициента выполнения; количество единиц изменений, которые необходимо обработать для выполнения синхронизации.|
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


