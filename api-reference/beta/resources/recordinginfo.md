---
title: Тип ресурса Рекордингинфо
description: Сведения о записи для участника.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d9e9a17a9afb197333e677547f3fa5dca22df9b2
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39637047"
---
# <a name="recordinginfo-resource-type"></a>Тип ресурса Рекордингинфо

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о записи для участника.

## <a name="properties"></a>Свойства

| Свойство        | Тип    | Описание|
|:----------------|:--------|:----------|
| initiatedBy     | [participantInfo](participantinfo.md) | Участник, который инициировал запись. |
| рекордингстатус | String | `unknown`Возможные значения: `notRecording`,, `recording`, или. `failed` |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "recordingStatus": "unknown | notRecording | recording | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
