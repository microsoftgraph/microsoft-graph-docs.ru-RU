---
title: Тип ресурса synchronizationProgress
description: Представляет ход выполнения synchronizationJob к завершению.
ms.openlocfilehash: 412b7754dac97a36efe082026ab360569c0fe789
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082431"
---
# <a name="synchronizationprogress-resource-type"></a>Тип ресурса synchronizationProgress

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет ход выполнения [synchronizationJob](synchronization-synchronizationjob.md) к завершению.

## <a name="properties"></a>Свойства

| Свойство                              | Тип      | Description    |
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
