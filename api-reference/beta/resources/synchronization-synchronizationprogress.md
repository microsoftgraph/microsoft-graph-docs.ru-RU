---
title: Тип ресурса synchronizationProgress
description: Представляет ход выполнения синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: f6f8f7cc5d0419a6f0e9203513db5b1452db1797
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131644"
---
# <a name="synchronizationprogress-resource-type"></a>Тип ресурса synchronizationProgress

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ход выполнения [синхронизации.](synchronization-synchronizationjob.md)

## <a name="properties"></a>Свойства

| Свойство                              | Тип      | Описание    |
|:--------------------------------------|:----------|:---------------|
|completedUnits|Int32|Числитель соотношения хода выполнения; количество уже обработанных единиц изменений.|
|progressObservationDateTime|DateTimeOffset|Время наблюдения за ходом выполнения как смещение в минутах от времени в UTC.|
|totalUnits|Int32|Коэффициент выполнения; количество единиц изменений, которые необходимо обработать для выполнения синхронизации.|
|units|Строка|Необязательное описание единиц.|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a>Представление в формате JSON

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


